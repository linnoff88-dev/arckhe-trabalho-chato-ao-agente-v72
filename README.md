# Entregue o trabalho chato a um agente (v7.2)

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


Curso aberto e gratuito do INEMA.CLUB, formato INEMA Learning v7.2, em PT, EN e ES.

- PT: https://inematds.github.io/trabalho-chato-ao-agente-v72/
- EN: https://inematds.github.io/trabalho-chato-ao-agente-v72/en/
- ES: https://inematds.github.io/trabalho-chato-ao-agente-v72/es/

Para dono de pequena empresa ou autÃ´nomo que usa ChatGPT/Claude no chat e nÃ£o programa: achar a tarefa chata da semana, escrever a ficha do agente, regras de seguranÃ§a (sÃ³ leitura, sÃ³ rascunho, login Ã© seu, dinheiro passa por vocÃª), modelo leve Ã— topo e um plano de 30 dias com diÃ¡rio de conferÃªncia. Toda prÃ¡tica tem o caminho no chat; o terminal (Claude Code ou Codex) Ã© opcional. Tudo pela assinatura, sem API paga.

## As aulas

1. Ache a tarefa chata certa
2. A ficha do agente em uma pÃ¡gina
3. O relatÃ³rio da semana sem abrir o painel
4. Contato novo vira rascunho, nunca envio
5. Nota e boleto: o dinheiro passa por vocÃª
6. Cliente novo: o checklist que para quando falha
7. Modelo leve para a rotina, topo para o difÃ­cil
8. Do primeiro agente Ã  pequena equipe em 30 dias

## O processo, do inÃ­cio ao fim

1. âš™ï¸ Criar a pasta: `~/.claude/skills/formato-curso-v72/scripts/novo-curso.sh ~/projetos/trabalho-chato-ao-agente-v72 "<nome>"`.
2. ðŸ§  Plano das aulas em `PLANO.md` (objetivo, diagrama, prÃ¡tica e conferidor de cada aula).
3. ðŸ§  ConteÃºdo em `conteudo/pt/curso.json` e `conteudo/pt/aulas/NN-<slug>.json`; conferidores testados com `python3 conferir.py <aula> --exemplo` e `--errado`.
4. ðŸ¤– Imagens: heros pelo Codex image_gen (`codex exec`, assinatura) e capa composta com tÃ­tulo em serifa (Playwright) â†’ `assets/img/`.
5. âš™ï¸ PortÃ£o PT: `python3 gerar.py && python3 validar.py --links` e `node ~/.claude/skills/formato-curso-v72/scripts/conferir-tela.cjs .`.
6. ðŸ¤– Revisor independente (Agent novo, persona do pÃºblico) â†’ nota em `~/projetos/wifi/scripts/revisor-nota.py`; corrigir e revisar de novo atÃ© â‰¥ 8.
7. ðŸ¤– TraduÃ§Ã£o: `python3 ~/.claude/skills/formato-curso-v72/scripts/traduzir.py . en es --publico "..."` (tradutor central, assinatura), glossÃ¡rio em `i18n/glossario.json`, cache em `i18n/<lang>.json`; depois `python3 i18n/localiza.py` (nomes, cidades, valores, datas e pastas do exemplo por mercado), o `traduzir.py` de novo (regrava do cache) e `python3 i18n/arquivos.py` (nomes de arquivo do conferidor); varreduras das Lessons.
8. âš™ï¸ PortÃ£o nos 3 idiomas: `python3 gerar.py --lang en|es`, `python3 validar.py --links --lang en|es`, `conferir-tela.cjs .`.
9. ðŸ¤– Um revisor por idioma (EN, ES).
10. âš™ï¸ Publicar: commit (autor `inematds`) + push; GitHub Pages da raiz da `main`.

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>