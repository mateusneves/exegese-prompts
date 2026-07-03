# 17. Tradução Literal

**Localização no trabalho:** Seção 4.3.2 — Tradução Literal

## O que este prompt gera
A tradução literal corrida de toda a perícope, construída a partir da análise gramatical palavra por palavra já produzida (prompt 16), mantendo a ordem e a estrutura do original tanto quanto a inteligibilidade permitir.

## Fontes recomendadas para esta seção
O resultado do prompt "16-analise-dos-versiculos" (cole-o como contexto), o texto original.

## Prompt (copie e cole no NotebookLM)

"""
Com base exclusivamente na análise gramatical palavra por palavra já produzida para a perícope **[PASSAGEM]** (cole aqui o resultado do prompt "Análise dos Versículos"), monte a seção **"Tradução Literal"**.

Junte as traduções literais de cada palavra/expressão, versículo por versículo, em uma tradução corrida da perícope inteira, mantendo:

- A ordem das palavras o mais próxima possível do texto original em [LÍNGUA ORIGINAL], mesmo que isso produza uma leitura mais rígida ou pouco natural em português.
- A escolha lexical já definida na análise gramatical (não troque por sinônimos mais fluentes nesta etapa — isso será feito na Tradução Dinâmica).
- A pontuação mínima necessária para separar orações, sem reorganizar a sintaxe.

Requisitos de formato:
- Apresente o texto corrido, dividido por número de versículo entre parênteses ou colchetes.
- Não adicione palavras que não estejam na análise gramatical fornecida (conectivos implícitos podem ser indicados entre colchetes, se necessário para a compreensão mínima).
- Extensão: a perícope completa, sem cortes.
"""

## Observações
Este prompt não requer fontes bibliográficas adicionais além do próprio resultado da Análise dos Versículos — é essencialmente uma tarefa de compilação/montagem, não de pesquisa. A "Tradução Dinâmica" (item do sumário sem prompt próprio) pode ser produzida manualmente por você a partir desta tradução literal, buscando fluência em português.
