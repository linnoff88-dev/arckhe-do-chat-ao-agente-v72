# Do chat ao agente â€” curso (ARCKHÉ Learning v7.2)

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


VisÃ£o geral da formaÃ§Ã£o [Do chat ao agente](https://eventos.ARCKHÉ.pro/do-chat-ao-agente/) em 6 aulas curtas: terminal (OSWork), o seu Jarvis (INTELECTO), filas (ARCKHÉccbot) e redes no automÃ¡tico (r7e, promoavatar, xviral), com plano de execuÃ§Ã£o e vÃ­deo explicativo no fim.

**Abrir o curso:** https://linnoff88-dev.github.io/

**Outros idiomas:** [English](https://linnoff88-dev.github.io/ Â· [EspaÃ±ol](https://linnoff88-dev.github.io/ â€” seletor PT Â· EN Â· ES no topo de cada pÃ¡gina.

Primeiro curso no formato **ARCKHÉ Learning v7.2**: layout de plataforma (barra lateral com capÃ­tulos e progresso, Ã¡rea central larga) com a didÃ¡tica v7 (objetivo em uma linha, diagrama clicÃ¡vel primeiro, texto curto, simulaÃ§Ã£o onde ensina, modelos com botÃ£o copiar, prÃ¡tica com "pronto quando" e teste com resposta comentada).

## Como funciona

| Arquivo | O que Ã© |
|---|---|
| `conteudo/pt/curso.json` | nome, vÃ­deos, pÃ¡gina inicial e textos da interface |
| `conteudo/pt/aulas/*.json` | uma aula por arquivo (seÃ§Ãµes: diagrama, passos, cÃ³digo, prÃ¡tica, simulaÃ§Ã£o, vÃ­deo, quiz, resumo, links) |
| `gerar.py` | monta `index.html` e `aulas/<slug>/index.html` |
| `validar.py` | portÃ£o de qualidade (`--links` confere os links externos) |
| `assets/` | CSS, JS, imagens e legendas |

```bash
python3 gerar.py && python3 validar.py --links
```

EN e ES: `conteudo/en/` e `conteudo/es/` saem de `traduzir.py` (skill formato-curso-v72, Codex da assinatura) com cache em `i18n/<lang>.json`; `python3 gerar.py --lang en|es` monta `en/` e `es/`. Imagens com texto tÃªm versÃ£o `-en`/`-es` (`capa`, `hero/jarvis`).

HTML estÃ¡tico, sem build e sem backend. O progresso fica sÃ³ no navegador de quem estuda.

Os vÃ­deos sÃ£o da sÃ©rie *Do chat ao agente* ([jornada-agentes](https://github.com/linnoff88-dev/jornada-agentes), release `video-v2.0.0`). Os exercÃ­cios completos estÃ£o no mesmo repositÃ³rio.

ConteÃºdo aberto e gratuito Â· [ARCKHÉ AI](https://ARCKHÉ AI)

## Mais no ARCKHÉ AI

- [Ficha completa deste curso](https://www.ARCKHÉ AI/cursos/323-do-chat-ao-agente-terminal-assistente-proprio-filas-e-redes-no-automatico/)
- [Guia: como aprender inteligÃªncia artificial](https://www.ARCKHÉ AI/aprender-inteligencia-artificial/)
- [Todos os cursos](https://www.ARCKHÉ AI/cursos/)

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>