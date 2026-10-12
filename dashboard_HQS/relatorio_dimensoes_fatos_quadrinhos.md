# Relatório de Dimensões e Fatos — Diagnóstico de Catálogo e Avaliações de Quadrinhos

Modelo estrela. Grão da fato: 1 linha por título de quadrinho.

## Tabela Fato: Fato_Quadrinhos

| Campo | Tipo | Observação |
|---|---|---|
| Titulo | Texto (chave) | Identifica o título |
| Classificação(0 a 100) | Número | Nota do título |
| N° de Páginas | Número | Páginas do título |
| Qtde de Volumes | Número | Volumes do título |
| Prêmios | Texto | Nulo = sem prêmio |
| Status | Texto | Ongoing / Completed / Hiatus / Cancelled |

Chaves estrangeiras (ligam às dimensões): Editora, Gênero, País, Formato,
Classificação Indicativa, Idioma, Tema, Ano.

## Dimensões

| Dimensão | Origem (coluna) | Atributos |
|---|---|---|
| Dim_Editora | Estudio/Editora | Nome da editora/estúdio |
| Dim_Genero | Gênero | Gênero do título |
| Dim_Pais | País de Origem | País (alguns valores compostos, ex. "South Korea / Japan") |
| Dim_Formato | Formato | Tankobon, Graphic Novel, Webtoon etc. |
| Dim_ClassificacaoIndicativa | Classificação Indicativa | All Ages, Teen+, Mature etc. |
| Dim_Idioma | Idioma | Idioma original |
| Dim_Tema | Tema (Estilo das Cores) | Full Color, Black & White etc. |
| Dim_Tempo | Ano de lançamento | Ano de lançamento |

## Fora do modelo estrela
Escritor e Artista ficam como atributos direto na fato (não viraram dimensão):
cada título tem só 1 escritor e 1 artista principal, sem relação
muitos-para-muitos nos dados.
