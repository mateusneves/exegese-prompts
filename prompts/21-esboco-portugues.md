# 21. Esboço em Português

**Localização no trabalho:** Seção 4.5.2 — Esboço em Português

## O que este prompt gera (e como se relaciona com o prompt 20)

O mesmo tipo de fluxograma lógico/retórico do prompt 20 (sequência, paralelismo, agrupamento de listas coordenadas, continuidade entre versículos distantes), mas construído **de forma independente, direto sobre o texto em português** — não é uma tradução mecânica do resultado do prompt 20. A IA deve analisar a sintaxe e a retórica da tradução portuguesa por si mesma, e não apenas substituir palavras hebraicas/gregas por palavras portuguesas em uma estrutura já pronta.

Isso é proposital: como o português tem ordem de palavras e estrutura de frase diferentes do hebraico/grego, a melhor forma de garantir que o diagrama em português seja natural e correto é a IA analisá-lo diretamente, e não herdar cegamente decisões estruturais tomadas para o idioma original. Depois de gerar os dois esboços (20 e 21), compare-os: se as relações de paralelismo e agrupamento identificadas forem semelhantes nos dois, isso é uma boa confirmação cruzada da análise; se forem diferentes em algum ponto, vale revisar qual dos dois capturou melhor a lógica do texto.

**Esta versão do prompt também pede a saída em [Mermaid](https://mermaid.js.org)**, para gerar um fluxograma visual de verdade no mermaid.live, assim como o prompt 20.

## Fontes recomendadas para esta seção
A tradução literal já produzida (prompt 17) ou o texto da perícope em uma tradução de sua preferência. Não é necessário colar o resultado do prompt 20.

## Prompt (copie e cole no NotebookLM)

"""
Com base no texto em português da perícope **[PASSAGEM]** abaixo (tradução literal ou de sua preferência), produza a seção **"Esboço em Português"** em formato de **código Mermaid** (diagrama do tipo `flowchart`).

Texto da perícope em português (cole aqui, versículo por versículo):
[TEXTO BÍBLICO]

Construa um fluxograma de fluxo lógico/retórico da perícope, no nível de cláusula/frase (agrupando palavras que formam uma unidade de sentido, não decompondo até a palavra isolada), seguindo estas regras de sintaxe Mermaid:

1. Comece o código com `flowchart TD` (top-down).
2. Cada cláusula vira um nó com um ID curto e o texto entre aspas duplas dentro de colchetes, ex.: `v10a["Ouvi a palavra do SENHOR"]`. Use IDs no padrão `v` + número do versículo + letra sequencial (v10a, v10b, v11a...).
3. **Sequência** (uma cláusula leva à seguinte): seta simples — `v10a --> v10b`.
4. **Paralelismo** (par de cláusulas paralelas, identificado por você a partir da estrutura retórica do texto em português): seta dupla — `v10c <--> v10d`.
5. **Agrupamento** (lista de itens sob uma afirmação governante): use um `subgraph`, com uma seta do nó anterior para o subgraph. Exemplo:
```
v11a["Estou farto / não me agrado"] --> lista11
subgraph lista11 [" "]
    v11i1["dos holocaustos de carneiros"]
    v11i2["e da gordura de animais cevados"]
    v11i3["e do sangue de novilhos"]
    v11i4["nem de cordeiros"]
    v11i5["nem de bodes"]
end
```
6. **Continuidade à distância** (uma afirmação distante continua conectada a algo várias linhas depois): use seta pontilhada com rótulo — `v11a -. "continua até v13" .-> v13e`.
7. Para identificar em que versículo cada nó está, adicione um comentário Mermaid antes do bloco correspondente: `%% Versículo 10`, `%% Versículo 11`, etc.

Requisitos de formato:
- Baseie a estrutura sintática e as relações de paralelismo exclusivamente no texto em português fornecido acima — não introduza elementos que não estejam nele.
- Use uma redação natural e gramaticalmente correta em português (não uma tradução literal desajeitada), mesmo que isso signifique reorganizar levemente a ordem das palavras em relação ao idioma original.
- Todo texto dentro de colchetes deve estar entre aspas duplas, sem aspas duplas dentro do próprio texto (use aspas simples se precisar citar algo dentro do rótulo).
- Gere **apenas o código Mermaid válido**, sem texto explicativo antes ou depois do bloco de código, para que eu possa copiar e colar diretamente em um visualizador.
- Ao final, como comentário Mermaid (`%%`), adicione uma frase explicando o principal padrão estrutural identificado no conjunto da perícope.
"""

## O que fazer com o resultado

1. Copie **só o código Mermaid** gerado (a partir de `flowchart TD` até o final).
2. Acesse **[mermaid.live](https://mermaid.live)** e cole o código no painel da esquerda ("Code"). O diagrama aparece renderizado automaticamente no painel da direita.
3. Se aparecer erro de sintaxe: geralmente é aspas dentro de um rótulo, parênteses ou dois-pontos sem estarem dentro de aspas, ou um nó com o mesmo ID repetido — corrija manualmente a linha indicada pelo erro.
4. Quando o diagrama estiver correto, use o botão de exportação do mermaid.live (canto superior direito) para baixar como PNG ou SVG, e insira essa imagem no seu documento Word na seção 4.5.2.

## Observações
Rode este prompt e o 20 em momentos diferentes (não precisa ser em sequência) e compare os dois diagramas renderizados ao final, em vez de gerar um a partir do outro. Pequenos ajustes manuais de sintaxe antes de renderizar são normais — o valor do prompt está na IA identificar corretamente a lógica das conexões, não na sintaxe Mermaid perfeita de primeira.
