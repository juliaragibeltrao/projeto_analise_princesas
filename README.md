# Diversidade sim. Protagonismo, nem sempre.

Um ensaio de dados sobre a diversidade racial/étnica das princesas da Disney (1937–2023)

Projeto de portfólio em ciência de dados / jornalismo de dados, desenvolvido com o objetivo de eventual submissão ao The Pudding.

## Pergunta de pesquisa

Como a diversidade racial/étnica das princesas da Disney mudou ao longo do tempo — e o que essa mudança revela sobre protagonismo, não só sobre presença?

## Perguntas que este projeto responde

- Quantos anos se passaram entre a primeira princesa da Disney e a primeira princesa não-branca?
- O surgimento de princesas não-brancas segue uma tendência contínua e crescente, ou aparece em surtos isolados?
- Existe uma diferença estrutural entre quem tem a etnia oficialmente declarada pela Disney e quem não tem — e o que isso revela sobre a ideia de "branquitude não marcada"?
- A recepção da crítica especializada e do público muda de acordo com a etnia da protagonista?
- A bilheteria mundial acompanha esse padrão — e os dados históricos de bilheteria são confiáveis o suficiente para sustentar essa comparação?
- O "boom multicultural" dos anos 1990 (Jasmine, Pocahontas, Mulan) representa um avanço real de protagonismo, ou uma diversificação predominantemente estética/comercial?
- (em aberto, próxima etapa) A assimetria observada entre os filmes também aparece dentro de cada filme, quando medida por tempo de fala e tempo de tela de cada personagem?

## Achados principais até o momento

**Branquitude não marcada.** Nenhuma das 7 princesas brancas/europeias do levantamento (Branca de Neve, Cinderela, Aurora, Ariel, Bela, Rapunzel, Merida) tem etnia declarada oficialmente pela Disney. As 8 princesas restantes vêm todas acompanhadas de comunicado oficial, entrevista de produção ou consultoria cultural que declara e justifica a etnia representada.

**Um surto, não uma tendência.** As princesas não-brancas aparecem em dois surtos concentrados — 1992–1998 e 2009–2023 — intercalados por décadas inteiras sem nenhum lançamento nessa linha, em vez de uma progressão contínua.

**Recepção não segue um padrão racial simples.** Apenas dois filmes do grupo têm aprovação da crítica abaixo de 60%: Pocahontas e Wish. Aladdin, Mulan, Moana e Raya têm notas tão altas quanto qualquer filme com princesa branca — o que descarta uma relação direta e simples entre etnia da protagonista e nota da crítica.

**Cuidado com a bilheteria histórica.** Filmes até 1991 (ex.: *A Bela Adormecida*) têm dados de bilheteria internacional incompletos nas bases usuas (Box Office Mojo/IMDb), o que pode distorcer comparações entre décadas se não for sinalizado.

## Dataset

Arquivo: `princesas_diversidade_dados.xlsx`

| Aba | Conteúdo |
| --- | --- |
| Dados | 15 princesas, com ano de lançamento, estúdio, etnia declarada, fonte da classificação, bilheteria, aprovação de crítica e público, prêmios e duração |
| Dicionário de Dados | Descrição de cada coluna |
| Notas Metodológicas | Registro de decisões difíceis, casos ambíguos e referências completas |
| Legenda | Instruções de uso da planilha |

## Metodologia de classificação de etnia

A etnia de cada personagem nunca foi inferida visualmente. Toda classificação é baseada em uma destas fontes, documentada linha a linha na planilha:

- Declaração oficial de estúdio ou comunicado de imprensa
- Entrevista com diretores, roteiristas ou produtores
- Literatura acadêmica revisada por pares
- Base histórica documentada (quando a personagem é inspirada em figura real)

Casos ambíguos (como Jasmine, cuja etnia nunca foi declarada de forma unívoca) são tratados como dado relevante em si, não como lacuna a esconder.

## Referências

- BENHAMOU, Eve. "From the Advent of Multiculturalism to the Erasure of Race: The Representation of Race Relations in Disney Animated Features (1995-2009)". *Exchanges: The Warwick Research Journal*, 2014.
- FOUGHT, Carmen; EISENHAUER, Karen. *Language and Gender in Children's Animated Films: Exploring Disney and Pixar*. Cambridge University Press, 2022.
- Gold Derby — ranking de tempo de tela das princesas Disney
- UCLA Library — guia de pesquisa sobre raça e etnia no universo Disney
- Entrevistas e comunicados oficiais: CBS News (Tiana, 2009), Geeks of Color (Asha, 2023), cobertura de imprensa sobre o Oceanic Story Trust (Moana, 2016)

Fontes completas e por personagem estão documentadas na aba "Notas Metodológicas" da planilha.

## Capturas de tela

Arquivo: `screenshot.gif`

Animação única reunindo as três etapas do protótipo:

- **Abertura** — as 15 princesas em ordem cronológica
- **Separação entre etnia nunca declarada e etnia oficialmente declarada**
- **Recepção da crítica e do público**, com *Pocahontas* e *Wish* destacadas

## Protótipo visual

Arquivo: `esboco_pudding_historia.html`

Protótipo de scrollytelling em D3.js, com um único gráfico que se transforma em 7 etapas conforme a rolagem da página (linha do tempo → separação por etnia declarada/não declarada → bilheteria → recepção crítica × público). Construído como esboço de estrutura para eventual pitch ao Pudding, não como peça final.

## Limitações conhecidas

- Dados de tempo de fala/tela por personagem individual ainda não integrados (Fought & Eisenhauer mede por gênero agregado, não por personagem)
- Coluna de prêmios coletada via IMDb, que mistura categorias oficiais e informais — recomenda-se confirmar cada prêmio relevante diretamente no site da Academia antes de uma versão final
- Classificação de etnia para Jasmine, Pocahontas e Mulan ainda depende parcialmente de wiki de fãs como fonte secundária

## Próximos passos

- Integrar dados de tempo de fala e tempo de tela por personagem
- Verificar prêmios diretamente nas fontes oficiais (Oscar, Globo de Ouro, Annie Awards)
- Refinar a tese central com base nos achados acima
- Pitch ao The Pudding via [pudding.cool/pitch](https://pudding.cool/pitch)
