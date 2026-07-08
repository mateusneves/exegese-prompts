# 16. Análise dos Versículos (Análise Gramatical)

**Localização no trabalho:** Seção 4.3.1 — Análise dos Versículos

## O que este prompt gera
Uma tabela palavra por palavra (ou, no caso de textos maiores, expressão por expressão) da perícope no idioma original, com a classificação gramatical de cada termo (classe de palavra, tempo verbal, pessoa, número, gênero, caso, raiz léxica) e sua tradução literal.

## Fontes recomendadas para esta seção
Um léxico hebraico ou grego (ex.: Holladay), uma gramática de referência do idioma. **Importante:** diferente das demais seções, aqui normalmente suas fontes carregadas no notebook serão só obras de referência (léxicos, dicionários, gramáticas) — elas não contêm o texto da sua perícope específica. Por isso, você mesmo precisa colar o texto da perícope no idioma original diretamente no prompt abaixo (copie de uma edição crítica como a BHS, para o Antigo Testamento, ou o Nestle-Aland/UBS, para o Novo Testamento).

## Prompt (copie e cole no NotebookLM)

```text
Com base no texto abaixo, em [LÍNGUA ORIGINAL], da perícope **[PASSAGEM]**, e utilizando exclusivamente o léxico e a gramática de referência carregados neste notebook para a classificação gramatical e o significado lexical, produza a seção **"Análise dos Versículos"**.

Texto da perícope no idioma original (cole aqui, versículo por versículo, indicando o número de cada um):
[TEXTO NO IDIOMA ORIGINAL]

Para cada versículo da perícope, monte uma tabela com três colunas:

1. **Palavra/expressão original** — a palavra ou expressão em [LÍNGUA ORIGINAL], na grafia correta (com pontuação vocálica, se hebraico).
2. **Análise gramatical** — classe de palavra (substantivo, verbo, partícula, adjetivo, etc.), e quando aplicável: para verbos, tronco/tema (ex. paal, hifil, nifal, piel — se hebraico; ou voz, modo, tempo — se grego), pessoa, número, gênero e o significado lexical básico entre parênteses; para substantivos, gênero, número e estado (absoluto/construto, se hebraico) e o significado lexical básico entre parênteses; para partículas e preposições, sua função e tradução possível.
3. **Tradução literal** — a tradução mais literal possível daquela palavra/expressão isolada, coerente com a análise gramatical.

Organize a tabela por versículo, com um cabeçalho de seção indicando "Versículo [número]" antes de cada bloco de palavras daquele versículo.

Requisitos de formato:
- Use o texto colado acima como base para as palavras e a ordem delas; use o léxico/gramática carregados neste notebook exclusivamente para a classificação gramatical e o significado lexical — não infira classificações gramaticais de memória.
- Cite em nota de rodapé (ABNT) o léxico ou gramática utilizado para as definições lexicais, na primeira ocorrência.
- Mantenha a ordem das palavras exatamente como aparecem no texto colado.
- Não pule nenhuma palavra do texto, incluindo conjunções, artigos e partículas.
```

## Observações
Esta é a seção mais mecânica e demorada de revisar manualmente. Antes de rodar o prompt, confira se colou o texto original correto e completo da perícope (recomendado copiar de uma edição crítica confiável, como BHS ou Nestle-Aland/UBS, para evitar erros de digitação). Depois, confira cuidadosamente a vocalização hebraica ou a acentuação grega geradas pela IA na tabela — erros de caractere são comuns em texto bíblico original processado por IA.
