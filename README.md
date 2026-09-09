# Bibliometria com VOSviewer e Bibliometrix: passo a passo (MirandasTech)

Manual em formato de slides (49) para mapear o campo da própria revisão na pós-graduação: o que a bibliometria mede e o que não mede (Manifesto de Leiden, DORA), os cinco tipos de rede (coautoria, coocorrência, citação, acoplamento bibliográfico, cocitação), contagem completa e fracionada, de onde vêm os dados e os limites de exportação de cada base (Web of Science, Scopus, Dimensions, Lens, PubMed, OpenAlex, Crossref); indicadores do corpus com `indicadores_bibliometricos.py` (produção por ano, fontes, autores, citações pelo Crossref, índice h do corpus); o VOSviewer (interface, Create Map, thesaurus, arquivos map/network/JSON) e o VOSviewer Online passo a passo com mapas reais abertos de verdade (`mapa_vosviewer.py`: coautoria, termos, fontes, acoplamento); Bibliometrix/biblioshiny e CiteSpace; a seção de método bibliométrico, erros comuns, checklist, glossário com popovers e referências. Corpus real e aberto de 236 documentos exportado do OpenAlex em 09/09/2026; capturas reais e datadas sem login.

**Manual on-line:** https://bibliometria.mirandastech.com.br/ · **PDF:** https://bibliometria.mirandastech.com.br/manual.pdf

Manuais irmãos: **Análise de dados** — https://dados.mirandastech.com.br/ · **Git e GitHub** — https://git.mirandastech.com.br/ · **LaTeX com Overleaf e abnTeX2** — https://latex.mirandastech.com.br/ · **Busca em bases científicas** — https://busca.mirandastech.com.br/ · **Revisão sistemática com PRISMA 2020** — https://prisma.mirandastech.com.br/ · **Zotero** — https://zotero.mirandastech.com.br/ · **Metodologia** — https://metodologia.mirandastech.com.br/ · **Gemini Notebook** — https://notebook.mirandastech.com.br/ · **Uso de IA na pesquisa** — https://manual.mirandastech.com.br/ · **Plugin Pesquisa (Claude e Codex)** — https://plugin.mirandastech.com.br/ · Hub: https://www.mirandastech.com.br/pesquisa

| Pasta | O que há |
|---|---|
| `manual/` | deck HTML autônomo, PDF, fonte do artefato e `fatos_verificados.md` (fontes, versões, execuções e mapas conferidos em 09/09/2026) |
| `site/` | o que o servidor serve (`index.html`, `manual.pdf`) |
| `capturas/` | 26 capturas reais, 09/09/2026 (páginas públicas; VOSviewer Online com os mapas do corpus; 2 figuras de terminal com saídas reais; 1 figura gerada por script) |
| `exemplo/` | o corpus real (`corpus.csv`, 236 registros do OpenAlex), o enriquecimento do Crossref, os mapas gerados (map/network/JSON) e os indicadores — para reproduzir e abrir no VOSviewer |
| `scripts/indicadores_bibliometricos.py` | total, período, produção por ano (figura por script), fontes, autores, tipos, acesso aberto, mais citados e índice h do corpus |
| `scripts/mapa_vosviewer.py` | redes de coautoria, termos, fontes e acoplamento bibliográfico nos formatos do VOSviewer (map + network) e do VOSviewer Online (JSON) |
| `scripts/gerar_deck.py` | regenera HTML e PDF a partir do fonte |
| `skills/bibliometria-vosviewer/` | skill do agente (cópia sincronizada do plugin Pesquisa MirandasTech) |
| `Dockerfile` · `Caddyfile` · `railway.json` | deploy estático (Caddy) |
| `.github/workflows/verificar.yml` | CI: integridade do deck e capturas referenciadas |

## Os manuais juntos
Este manual cobre o **mapeamento do campo**: o corpus vem da busca registrada (manual de busca), os indicadores e os mapas ilustram a revisão (manual de revisão sistemática), as figuras entram no LaTeX e a versão no Git. No plugin **Pesquisa MirandasTech** (`pesquisa-mirandastech`), a skill `bibliometria-vosviewer` gera os arquivos e explica cada rede; o aluno escolhe o corpus, os limiares e a interpretação; nenhum indicador serve para «avaliar» pessoas.

## Como citar
MATIAS, J. P. M. *Bibliometria com VOSviewer e Bibliometrix: passo a passo.* MirandasTech, v1.0, set. 2026. CC BY 4.0.

## Declaração de uso de IA
Escrito com assistência de IA (Claude, Anthropic) na estruturação, redação, automação das capturas e execução dos scripts. Versões, limites, nomes de botões e referências conferidos nas fontes oficiais, no manual do VOSviewer 1.6.20 e em execuções reais em 09/09/2026 (lista em `manual/fatos_verificados.md`); nenhuma captura foi feita com login; o VOSviewer desktop e o Bibliometrix não foram executados e são descritos pela documentação oficial. O autor responde integralmente pelo conteúdo. VOSviewer/CWTS, Bibliometrix, Clarivate, Elsevier, Digital Science, Cambia/Lens, OpenAlex/OurResearch, Crossref e os demais serviços citados são marcas e projetos de terceiros; este manual não tem vínculo com eles.
