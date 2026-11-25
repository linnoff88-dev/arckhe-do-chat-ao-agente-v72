# Do chat ao agente ê¢â¬â curso (ARCKHê Learning v7.2)

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


VisêÂ£o geral da formaêÂ§êÂ£o [Do chat ao agente](https://eventos.ARCKHê.pro/do-chat-ao-agente/) em 6 aulas curtas: terminal (OSWork), o seu Jarvis (INTELECTO), filas (ARCKHêccbot) e redes no automêÂ¡tico (r7e, promoavatar, xviral), com plano de execuêÂ§êÂ£o e vêÂ­deo explicativo no fim.

**Abrir o curso:** https://linnoff88-dev.github.io/

**Outros idiomas:** [English](https://linnoff88-dev.github.io/ êÂ· [EspaêÂ±ol](https://linnoff88-dev.github.io/ ê¢â¬â seletor PT êÂ· EN êÂ· ES no topo de cada pêÂ¡gina.

Primeiro curso no formato **ARCKHê Learning v7.2**: layout de plataforma (barra lateral com capêÂ­tulos e progresso, êÂ¡rea central larga) com a didêÂ¡tica v7 (objetivo em uma linha, diagrama clicêÂ¡vel primeiro, texto curto, simulaêÂ§êÂ£o onde ensina, modelos com botêÂ£o copiar, prêÂ¡tica com "pronto quando" e teste com resposta comentada).

## Como funciona

| Arquivo | O que êÂ© |
|---|---|
| `conteudo/pt/curso.json` | nome, vêÂ­deos, pêÂ¡gina inicial e textos da interface |
| `conteudo/pt/aulas/*.json` | uma aula por arquivo (seêÂ§êÂµes: diagrama, passos, cêÂ³digo, prêÂ¡tica, simulaêÂ§êÂ£o, vêÂ­deo, quiz, resumo, links) |
| `gerar.py` | monta `index.html` e `aulas/<slug>/index.html` |
| `validar.py` | portêÂ£o de qualidade (`--links` confere os links externos) |
| `assets/` | CSS, JS, imagens e legendas |

```bash
python3 gerar.py && python3 validar.py --links
```

EN e ES: `conteudo/en/` e `conteudo/es/` saem de `traduzir.py` (skill formato-curso-v72, Codex da assinatura) com cache em `i18n/<lang>.json`; `python3 gerar.py --lang en|es` monta `en/` e `es/`. Imagens com texto têÂªm versêÂ£o `-en`/`-es` (`capa`, `hero/jarvis`).

HTML estêÂ¡tico, sem build e sem backend. O progresso fica sêÂ³ no navegador de quem estuda.

Os vêÂ­deos sêÂ£o da sêÂ©rie *Do chat ao agente* ([jornada-agentes](https://github.com/linnoff88-dev/jornada-agentes), release `video-v2.0.0`). Os exercêÂ­cios completos estêÂ£o no mesmo repositêÂ³rio.

ConteêÂºdo aberto e gratuito êÂ· [ARCKHê AI](https://ARCKHê AI)

## Mais no ARCKHê AI

- [Ficha completa deste curso](https://www.ARCKHê AI/cursos/323-do-chat-ao-agente-terminal-assistente-proprio-filas-e-redes-no-automatico/)
- [Guia: como aprender inteligêÂªncia artificial](https://www.ARCKHê AI/aprender-inteligencia-artificial/)
- [Todos os cursos](https://www.ARCKHê AI/cursos/)

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>