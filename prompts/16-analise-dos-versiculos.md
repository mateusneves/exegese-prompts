# 16. Análise dos Versículos (Análise Gramatical)

**Localização no trabalho:** Seção 4.3.1 — Análise dos Versículos

## O que este prompt gera
Uma tabela palavra por palavra (ou, no caso de textos maiores, expressão por expressão) da perícope no idioma original, com a classificação gramatical de cada termo (classe de palavra, tempo verbal, pessoa, número, gênero, caso, raiz léxica) e sua tradução literal.

## Fontes recomendadas para esta seção
O texto original (BHS para hebraico, Nestle-Aland/UBS para grego), um léxico hebraico ou grego (ex.: Holladay), uma gramática de referência do idioma.

## Prompt (copie e cole no NotebookLM)

"""
Com base exclusivamente nas fontes carregadas neste notebook (texto original em [LÍNGUA ORIGINAL] e léxico/gramática de referência), produza a seção **"Análise dos Versículos"** de um trabalho de exegese sobre a perícope **[PASSAGEM]**.

Para cada versículo da perícope, monte uma tabela com três colunas:

1. **Palavra/expressão original** — a palavra ou expressão em [LÍNGUA ORIGINAL], na grafia correta (com pontuação vocálica, se hebraico).
2. **Análise gramatical** — classe de palavra (substantivo, verbo, partícula, adjetivo, etc.), e quando aplicável: para verbos, tronco/tema (ex. paal, hifil, nifal, piel — se hebraico; ou voz, modo, tempo — se grego), pessoa, número, gênero e o significado lexical básico entre parênteses; para substantivos, gênero, número e estado (absoluto/construto, se hebraico) e o significado lexical básico entre parênteses; para partículas e preposições, sua função e tradução possível.
3. **Tradução literal** — a tradução mais literal possível daquela palavra/expressão isolada, coerente com a análise gramatical.

Organize a tabela por versículo, com um cabeçalho de seção indicando "Versículo [número]" antes de cada bloco de palavras daquele versículo.

Requisitos de formato:
- Baseie toda classificação gramatical exclusivamente no texto original e no léxico/gramática carregados neste notebook — não infira classificações gramaticais de memória.
- Cite em nota de rodapé (ABNT) o léxico ou gramática utilizado para as definições lexicais, na primeira ocorrência.
- Mantenha a ordem das palavras exatamente como aparecem no texto original.
- Não pule nenhuma palavra do texto, incluindo conjunções, artigos e partículas.
"""

## Observações
Esta é a seção mais mecânica e demorada de revisar manualmente — confira cuidadosamente a vocalização hebraica ou a acentuação grega gerada pela IA, pois erros de caractere são comuns em texto bíblico original processado por IA.
