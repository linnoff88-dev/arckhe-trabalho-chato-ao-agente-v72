ï»¿# Entregue o trabalho chato a um agente (v7.2)

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


Curso aberto e gratuito do INEMA.CLUB, formato INEMA Learning v7.2, em PT, EN e ES.

- PT: https://inematds.github.io/trabalho-chato-ao-agente-v72/
- EN: https://inematds.github.io/trabalho-chato-ao-agente-v72/en/
- ES: https://inematds.github.io/trabalho-chato-ao-agente-v72/es/

Para dono de pequena empresa ou autêÂ´nomo que usa ChatGPT/Claude no chat e nêÂ£o programa: achar a tarefa chata da semana, escrever a ficha do agente, regras de seguranêÂ§a (sêÂ³ leitura, sêÂ³ rascunho, login êÂ© seu, dinheiro passa por vocêÂª), modelo leve êâ topo e um plano de 30 dias com diêÂ¡rio de conferêÂªncia. Toda prêÂ¡tica tem o caminho no chat; o terminal (Claude Code ou Codex) êÂ© opcional. Tudo pela assinatura, sem API paga.

## As aulas

1. Ache a tarefa chata certa
2. A ficha do agente em uma pêÂ¡gina
3. O relatêÂ³rio da semana sem abrir o painel
4. Contato novo vira rascunho, nunca envio
5. Nota e boleto: o dinheiro passa por vocêÂª
6. Cliente novo: o checklist que para quando falha
7. Modelo leve para a rotina, topo para o difêÂ­cil
8. Do primeiro agente êÂ  pequena equipe em 30 dias

## O processo, do inêÂ­cio ao fim

1. ê¢Å¡â¢ê¯Â¸Â Criar a pasta: `~/.claude/skills/formato-curso-v72/scripts/novo-curso.sh ~/projetos/trabalho-chato-ao-agente-v72 "<nome>"`.
2. ê°Å¸Â§Â  Plano das aulas em `PLANO.md` (objetivo, diagrama, prêÂ¡tica e conferidor de cada aula).
3. ê°Å¸Â§Â  ConteêÂºdo em `conteudo/pt/curso.json` e `conteudo/pt/aulas/NN-<slug>.json`; conferidores testados com `python3 conferir.py <aula> --exemplo` e `--errado`.
4. ê°Å¸Â¤â Imagens: heros pelo Codex image_gen (`codex exec`, assinatura) e capa composta com têÂ­tulo em serifa (Playwright) ê¢â â `assets/img/`.
5. ê¢Å¡â¢ê¯Â¸Â PortêÂ£o PT: `python3 gerar.py && python3 validar.py --links` e `node ~/.claude/skills/formato-curso-v72/scripts/conferir-tela.cjs .`.
6. ê°Å¸Â¤â Revisor independente (Agent novo, persona do pêÂºblico) ê¢â â nota em `~/projetos/wifi/scripts/revisor-nota.py`; corrigir e revisar de novo atêÂ© ê¢â°Â¥ 8.
7. ê°Å¸Â¤â TraduêÂ§êÂ£o: `python3 ~/.claude/skills/formato-curso-v72/scripts/traduzir.py . en es --publico "..."` (tradutor central, assinatura), glossêÂ¡rio em `i18n/glossario.json`, cache em `i18n/<lang>.json`; depois `python3 i18n/localiza.py` (nomes, cidades, valores, datas e pastas do exemplo por mercado), o `traduzir.py` de novo (regrava do cache) e `python3 i18n/arquivos.py` (nomes de arquivo do conferidor); varreduras das Lessons.
8. ê¢Å¡â¢ê¯Â¸Â PortêÂ£o nos 3 idiomas: `python3 gerar.py --lang en|es`, `python3 validar.py --links --lang en|es`, `conferir-tela.cjs .`.
9. ê°Å¸Â¤â Um revisor por idioma (EN, ES).
10. ê¢Å¡â¢ê¯Â¸Â Publicar: commit (autor `inematds`) + push; GitHub Pages da raiz da `main`.

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>