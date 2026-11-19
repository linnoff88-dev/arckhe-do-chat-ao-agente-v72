# Do chat ao agente â€” curso (INEMA Learning v7.2)

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


VisÃ£o geral da formaÃ§Ã£o [Do chat ao agente](https://eventos.inema.pro/do-chat-ao-agente/) em 6 aulas curtas: terminal (OSWork), o seu Jarvis (INTELECTO), filas (inemaccbot) e redes no automÃ¡tico (r7e, promoavatar, xviral), com plano de execuÃ§Ã£o e vÃ­deo explicativo no fim.

**Abrir o curso:** https://inematds.github.io/do-chat-ao-agente-v72/

**Outros idiomas:** [English](https://inematds.github.io/do-chat-ao-agente-v72/en/) Â· [EspaÃ±ol](https://inematds.github.io/do-chat-ao-agente-v72/es/) â€” seletor PT Â· EN Â· ES no topo de cada pÃ¡gina.

Primeiro curso no formato **INEMA Learning v7.2**: layout de plataforma (barra lateral com capÃ­tulos e progresso, Ã¡rea central larga) com a didÃ¡tica v7 (objetivo em uma linha, diagrama clicÃ¡vel primeiro, texto curto, simulaÃ§Ã£o onde ensina, modelos com botÃ£o copiar, prÃ¡tica com "pronto quando" e teste com resposta comentada).

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

Os vÃ­deos sÃ£o da sÃ©rie *Do chat ao agente* ([jornada-agentes](https://github.com/inematds/jornada-agentes), release `video-v2.0.0`). Os exercÃ­cios completos estÃ£o no mesmo repositÃ³rio.

ConteÃºdo aberto e gratuito Â· [INEMA.CLUB](https://inema.club)

## Mais no INEMA.CLUB

- [Ficha completa deste curso](https://www.inema.club/cursos/323-do-chat-ao-agente-terminal-assistente-proprio-filas-e-redes-no-automatico/)
- [Guia: como aprender inteligÃªncia artificial](https://www.inema.club/aprender-inteligencia-artificial/)
- [Todos os cursos](https://www.inema.club/cursos/)

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>