# diagnostico-catalogo-quadrinhos

Diagnóstico de Catálogo e Avaliações de Quadrinhos — projeto de analytics em
Power BI sobre um catálogo de 10.000 títulos (mangás, HQs ocidentais,
manhuas e webtoons).

## Dataset
`comic_books_10000_dataset.csv` — 10.000 linhas, 17 colunas: editora,
escritor, artista, gênero, país de origem, formato, nota, status, faixa
etária, prêmios, páginas e volumes.

## Estrutura
- `PEA_Diagnostico_Quadrinhos_Claudio.docx` — Planejamento Estratégico
  (contexto, objetivo, perguntas analíticas, dados, indicadores, entregas,
  público, riscos e próximos passos)
- `relatorio_dimensoes_fatos_quadrinhos.md` — modelo estrela (1 fato +
  8 dimensões)
- `comic_books_10000_dataset.csv` — dataset bruto
- `.pbix` — relatório Power BI (dashboard)

## Perguntas analíticas
1. Quais editoras concentram mais títulos e qual a nota média de cada uma?
2. Como o gênero varia entre os países de origem?
3. Quais editoras têm maior % de títulos premiados?
4. Como a nota média varia por faixa etária?
5. Como os títulos se distribuem por status em cada editora?
6. Quais são os 10 quadrinhos mais bem avaliados?
7. Existe relação entre número de páginas e de volumes?

## Autor
Cláudio Vinícius Coelho Barros
