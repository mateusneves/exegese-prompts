# 19. Análise Manuscritológica

**Localização no trabalho:** Seção 4.4 — Análise Manuscritológica

## ⚠️ Seção de alto risco — leia antes de usar

Esta é provavelmente a seção mais delicada de toda a biblioteca. Uma sigla de manuscrito trocada, uma variante "inventada" ou uma data errada são erros graves, difíceis de perceber numa revisão rápida e sérios num trabalho acadêmico. Por isso, este prompt é rígido quanto à origem dos dados: a IA só pode trabalhar com variantes textuais que estejam em algo que você forneceu (aparato crítico colado ou nota textual de um comentário carregado) — nunca "de memória".

## De onde vem o aparato crítico (isto NÃO está nos seus léxicos/gramáticas/Paroschi)

O aparato crítico é o conjunto de notas técnicas de rodapé de uma **edição crítica** do texto original — BHS (Antigo Testamento) ou Nestle-Aland/UBS (Novo Testamento). Léxicos, gramáticas e o manual de Paroschi tratam de *método* e *vocabulário*, não reproduzem o aparato de um versículo específico. Duas formas de conseguir os dados desta seção:

1. **Aparato bruto de uma edição crítica** — para o Novo Testamento (grego), o **aparato do SBLGNT** (Michael Holmes) é uma opção confiável, estática e gratuita: baixe o pacote "SBLGNT Text and Apparatus" em sblgnt.com/download/ e carregue-o como fonte no notebook (ou copie direto os trechos da sua perícope para colar no prompt). **Atenção à natureza desse aparato:** ele não compara manuscritos antigos individualmente (não traz siglas como 𝔓⁴⁶, ℵ, B, D) — ele registra onde a SBLGNT diverge de quatro edições críticas modernas (WH = Westcott-Hort, Treg = Tregelles, NIV = texto grego por trás da NIV, RP = Textform Bizantino de Robinson-Pierpont), citando o NA apenas quando ele diverge da NIV. É uma comparação entre edições, não entre testemunhas manuscritas primárias — ainda assim, é dado real e citável, só precisa ficar claro no texto qual dos dois tipos de aparato foi usado. Para o Antigo Testamento (hebraico) ou para um aparato de manuscritos primários no NT (NA28/UBS completo), você ainda depende de uma edição crítica tradicional (BHS/NA28 impressa ou digital, softwares como Logos/Accordance/BibleWorks).
2. **Notas textuais de um comentário técnico** — se você não tiver nenhum aparato, mas tiver carregado um comentário que discute variantes textuais da perícope em suas próprias notas (comum em séries acadêmicas como Word Biblical Commentary), a IA pode se basear nisso — citando o comentarista como fonte da variante, sem fingir ter consultado a BHS/NA28/SBLGNT diretamente.

Se você não tiver nenhuma das duas coisas, é mais honesto pular ou simplificar bastante esta seção do que arriscar dados fabricados.

**Notação do aparato do SBLGNT**, caso o utilize: leitura do texto em negrito, seguida de `]` e da(s) variante(s); `•` separa variantes diferentes no mesmo versículo; `;` separa múltiplas leituras variantes na mesma unidade; `+` = a leitura seguinte é um acréscimo; `–` = omissão; `⸀`/`⸂ ⸃` no texto apontam para a nota correspondente no aparato; abreviações WH/Treg/NIV/RP/NA/TR/Holmes/Greeven identificam a edição. Não confunda essas siglas com a notação de manuscritos primários (𝔓, ℵ, A, B, D, it, vg, syr, cop) usada no NA28/UBS completo — são dois sistemas diferentes.

## Fontes recomendadas para esta seção
Obra(s) de crítica textual (Paroschi, para os critérios de avaliação), e pelo menos uma das fontes de dados de variantes descritas acima — para o NT, o pacote "SBLGNT Text and Apparatus" (sblgnt.com/download/) carregado como fonte é uma boa opção estática e gratuita.

## Prompt (copie e cole no NotebookLM)

"""
Com base **exclusivamente** nos dados fornecidos abaixo e nas fontes carregadas neste notebook, redija a seção **"Análise Manuscritológica"** de um trabalho de exegese sobre a perícope **[PASSAGEM]**, texto em **[LÍNGUA ORIGINAL]**.

Texto da perícope no idioma original (cole aqui, versículo por versículo):
[TEXTO NO IDIOMA ORIGINAL]

Dados sobre variantes textuais desta perícope — cole AO MENOS UMA das duas opções abaixo (ou ambas):
(a) Entradas do aparato crítico (BHS ou Nestle-Aland/UBS) correspondentes a esta perícope, coladas exatamente como aparecem na edição, incluindo siglas de manuscritos/versões:
[APARATO CRÍTICO DA PERÍCOPE — se disponível]
(b) Se você não tiver o aparato bruto, identifique aqui quais comentários carregados neste notebook trazem notas textuais sobre esta perícope, para que a IA busque essa informação neles:
[COMENTÁRIOS COM NOTAS TEXTUAIS SOBRE ESTA PERÍCOPE — se aplicável]

Para cada variante textual identificada — seja no aparato colado, seja nas notas textuais dos comentários indicados:

1. Identifique o versículo e a expressão em que ocorre a variante, e a fonte de onde a variante foi extraída (aparato colado ou comentário específico, com nota de rodapé ABNT neste segundo caso).
2. Descreva a variante (leitura do texto-base versus leitura(s) alternativa(s)), preservando exatamente as siglas e a informação fornecidas na fonte — não troque, não "modernize" e não complete siglas ou dados que não estejam explícitos na fonte utilizada.
3. Avalie a variante à luz dos critérios de crítica textual (testemunho externo — idade, distribuição geográfica, qualidade dos manuscritos; testemunho interno — qual leitura explica melhor o surgimento das demais, qual se harmoniza com o estilo do autor), com base no que a(s) obra(s) de crítica textual carregadas dizem sobre esses critérios em geral.
4. Conclua se a variante tem impacto relevante sobre a interpretação, a teologia ou a tradução da perícope, ou se é uma diferença menor sem consequência interpretativa.

Ao final, escreva um parágrafo de síntese avaliando o grau de estabilidade textual da perícope, com base somente nas variantes efetivamente identificadas nas fontes fornecidas.

Requisitos de formato:
- **Regra inegociável:** se uma variante, sigla, manuscrito, data ou leitura não estiver explicitamente presente no aparato colado ou em um comentário carregado que a discuta, você não deve mencioná-la, especulá-la ou preenchê-la com conhecimento geral — mesmo que pareça uma informação plausível ou comum em crítica textual.
- Se nem aparato crítico nem notas textuais de comentários estiverem disponíveis para esta perícope, diga isso explicitamente e não prossiga com a análise de variantes (pode, se fizer sentido, apenas declarar que a estabilidade textual da perícope não pôde ser verificada por falta de acesso a uma edição crítica).
- Preserve a notação técnica exatamente como fornecida na fonte utilizada, sem misturar sistemas diferentes: (i) aparato da BHS para o Antigo Testamento — ex.: 𝔊 Septuaginta, 𝔖 Peshita, 𝔗 Targum, 𝔙 Vulgata, 𝔔 manuscritos de Qumran; (ii) aparato de manuscritos primários do NA28/UBS para o Novo Testamento — ex.: 𝔓⁴⁶, ℵ, A, B, D, it, vg, syr, cop; (iii) aparato de edições do SBLGNT para o Novo Testamento — abreviações WH, Treg, NIV, RP, NA (indicando edições, não manuscritos) e símbolos `]`, `•`, `;`, `+`, `–`. Se a fonte for o SBLGNT, diga isso explicitamente no texto (ex.: "conforme o aparato do SBLGNT, que compara a edição com WH, Treg, NIV e RP") para não dar a impressão de que se trata de uma comparação com manuscritos primários.
- Redija em prosa acadêmica corrida, em português, terceira pessoa, com citações em nota de rodapé no padrão ABNT.
"""

## Observações
Depois de gerar o resultado, confira manualmente cada sigla e cada leitura mencionada contra a fonte original (o aparato que você colou ou o comentário citado) — não contra a "memória" da IA. Se notar qualquer variante, data ou manuscrito que não esteja na fonte indicada, é sinal de que a IA extrapolou e o trecho deve ser removido ou reescrito manualmente.
