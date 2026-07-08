# 18. Análise das Versões

**Localização no trabalho:** Seção 4.3.4 — Análise das Versões

## O que este prompt gera
Uma tabela comparativa, versículo por versículo, entre a tradução literal produzida e as principais versões da Bíblia em português, seguida de uma análise crítica das diferenças relevantes de tradução.

## Fontes recomendadas para esta seção
Várias traduções da Bíblia em português (ex.: ACF, ARA, ARC, NVI, NAA, NTLH, KJA), a tradução literal já produzida (prompt 17).

## Prompt (copie e cole no NotebookLM)

```text
Com base exclusivamente na tradução literal já produzida para a perícope **[PASSAGEM]** (cole-a aqui como referência) e nas versões da Bíblia em português disponíveis neste notebook, produza a seção **"Análise das Versões"**.

Primeiro, monte uma tabela comparativa, versículo por versículo, com a seguinte estrutura: uma coluna "Literal" (com o texto da tradução literal já produzida) e uma coluna para cada versão da Bíblia disponível (identificada pela sigla da versão, ex.: ACF, ARA, ARC, NVI), trazendo o texto de cada versão para aquele versículo.

Em seguida, escreva um comentário analítico, versículo por versículo, destacando:

1. Diferenças relevantes de tradução entre as versões e a tradução literal (omissões, escolhas lexicais divergentes, paráfrases, interpretações teológicas embutidas na tradução).
2. Versões que se destacam por serem mais parafrásticas ou mais interpretativas do que o texto original permite, e versões que se mantêm mais próximas do sentido literal.
3. Uma avaliação, ao final, indicando quais versões você (redator do comentário) considera mais fiéis ao texto original nesta perícope específica, e quais apresentam problemas de tradução, com base na comparação feita.

Requisitos de formato:
- Além da comparação entre as versões, traga também, quando disponíveis nas fontes, opiniões de pelo menos 5 a 7 comentaristas ou autores diferentes sobre as escolhas de tradução mais relevantes da perícope — mais de um autor pode opinar de forma parecida ou complementar, isso é desejável, pois dá mais opções para você escolher e remover manualmente na revisão final, sem esvaziar a seção. Se as fontes não trouxerem tantas vozes diferentes sobre tradução, utilize o máximo disponível e diga isso explicitamente.
- Utilize majoritariamente citação indireta (paráfrase), mas inclua ao menos 4 citações diretas (transcrição literal entre aspas) de comentaristas ao longo da análise, quando as fontes permitirem.
- Nomeie explicitamente o autor no corpo do texto (não apenas na nota de rodapé) sempre que atribuir uma opinião a ele — use fórmulas como "Segundo [Autor]...", "[Autor] afirma que...", "Conforme [Autor]...".
- Redija a parte analítica em prosa acadêmica corrida, em português, terceira pessoa.
- Organize a análise por número de versículo, com subtítulo "Versículo [número]" antes de cada bloco de comentário.
- Ao final, inclua um parágrafo de síntese geral sobre a confiabilidade das versões analisadas para esta perícope.
- Indique em nota de rodapé (ABNT) a edição e o ano de cada versão bíblica utilizada, na primeira menção.
```

## Observações
Quanto mais versões você carregar no notebook, mais rica fica esta seção — o modelo de referência (Isaías) utiliza catorze versões diferentes, incluindo três de Portugal.
