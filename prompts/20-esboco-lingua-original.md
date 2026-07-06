# 20. Esboço na Língua Original (Hebraico/Grego)

**Localização no trabalho:** Seção 4.5.1 — Esboço em Hebraico (ou Grego, conforme o Testamento)

## O que este prompt gera (e o que ele NÃO é)

**Não é** uma árvore de subordinação gramatical (oração principal à esquerda, subordinadas recuadas progressivamente à direita) — essa é uma técnica de diagramação diferente e não é a que o modelo de referência usa. **É** um **fluxograma de fluxo lógico e retórico da perícope**, no nível de cláusula/frase (não palavra por palavra), com quatro relações visuais:

1. **Sequência** — uma afirmação leva à/é seguida pela próxima no argumento do texto.
2. **Paralelismo** — duas cláusulas que dizem essencialmente a mesma coisa com palavras diferentes, ou que formam um par (dois vocativos, duas ordens sinônimas).
3. **Agrupamento** — uma lista de itens coordenados (objetos de um mesmo verbo, elaborações de uma mesma ideia) reunidos sob uma única afirmação governante.
4. **Continuidade à distância** — uma afirmação (ex.: "diz o SENHOR") continua "governando" o que vem várias linhas depois, mesmo com material intermediário no meio.

No modelo de referência (Isaías 1.10-20): "estou farto" aponta para um grupo de cinco itens de sacrifício (carneiros, gordura, sangue, cordeiros, bodes); "Sodoma" e "Gomorra" formam um par paralelo; e "diz o SENHOR" (v.11) continua governando o texto até "não continueis a trazer ofertas vãs" (v.13).

**Esta versão do prompt pede a saída em [Mermaid](https://mermaid.js.org)**, uma linguagem de diagrama em texto — assim você consegue transformar o resultado num fluxograma visual de verdade (caixas e setas), sem precisar de uma IA que gera imagem e sem precisar redesenhar tudo à mão.

## Fontes recomendadas para esta seção
Texto original, a análise gramatical já produzida (prompt 16), uma gramática de referência.

## Prompt (copie e cole no NotebookLM)

"""
Com base exclusivamente no texto original em [LÍNGUA ORIGINAL] e na análise gramatical já produzida para a perícope **[PASSAGEM]** (cole-a aqui como referência), produza a seção **"Esboço em [LÍNGUA ORIGINAL]"** em formato de **código Mermaid** (diagrama do tipo `flowchart`).

Construa um fluxograma de fluxo lógico/retórico da perícope, no nível de cláusula/frase (agrupando palavras que formam uma unidade de sentido, não decompondo até a palavra isolada), seguindo estas regras de sintaxe Mermaid:

1. Comece o código com `flowchart TD` (top-down).
2. Cada cláusula vira um nó com um ID curto e o texto entre aspas duplas dentro de colchetes, ex.: `v10a["שִׁמְעוּ דְבַר־יְהוָה"]`. Use IDs no padrão `v` + número do versículo + letra sequencial (v10a, v10b, v11a...).
3. **Sequência** (uma cláusula leva à seguinte): seta simples — `v10a --> v10b`.
4. **Paralelismo** (par de cláusulas paralelas): seta dupla — `v10c <--> v10d`.
5. **Agrupamento** (lista de itens sob uma afirmação governante): use um `subgraph`, com o nome da afirmação governante como rótulo do subgraph, e uma seta do nó anterior para o subgraph. Exemplo:
```
v11a["שָׁבַעְתִּי / לֹא חָפַצְתִּי"] --> lista11
subgraph lista11 [" "]
    v11i1["עֹלוֹת אֵילִים"]
    v11i2["וְחֵלֶב מְרִיאִים"]
    v11i3["וְדַם פָּרִים"]
    v11i4["וּכְבָשִׂים"]
    v11i5["וְעַתּוּדִים"]
end
```
6. **Continuidade à distância** (uma afirmação distante continua conectada a algo várias linhas depois): use seta pontilhada com rótulo — `v11a -. "continua até v13" .-> v13e`.
7. Para identificar em que versículo cada nó está, adicione um comentário Mermaid antes do bloco correspondente: `%% Versículo 10`, `%% Versículo 11`, etc.

Requisitos de formato:
- Baseie a estrutura sintática e as relações de paralelismo exclusivamente na análise gramatical fornecida e no texto original — não introduza elementos que não estejam na fonte.
- Mantenha o texto dos nós no idioma original ([LÍNGUA ORIGINAL]).
- Todo texto dentro de colchetes deve estar entre aspas duplas, sem aspas duplas dentro do próprio texto (se o texto original tiver aspas, substitua por aspas simples).
- Gere **apenas o código Mermaid válido**, sem texto explicativo antes ou depois do bloco de código, para que eu possa copiar e colar diretamente em um visualizador.
- Ao final, como comentário Mermaid (`%%`), adicione uma frase explicando o principal padrão estrutural identificado no conjunto da perícope.
"""

## O que fazer com o resultado

1. Copie **só o código Mermaid** gerado (a partir de `flowchart TD` até o final — não inclua nenhum texto explicativo que a IA tenha adicionado antes/depois, se houver).
2. Acesse **[mermaid.live](https://mermaid.live)** e cole o código no painel da esquerda ("Code"). O diagrama aparece renderizado automaticamente no painel da direita.
3. Se aparecer erro de sintaxe: geralmente é aspas dentro de um rótulo, parênteses ou dois-pontos sem estarem dentro de aspas, ou um nó com o mesmo ID repetido — corrija manualmente a linha indicada pelo erro.
4. Quando o diagrama estiver correto, use o botão de exportação do mermaid.live (canto superior direito) para baixar como PNG ou SVG, e insira essa imagem no seu documento Word na seção 4.5.1.

## Observações
Espere ter que fazer pequenos ajustes manuais na sintaxe Mermaid antes de renderizar sem erros — isso é normal e rápido de corrigir. O valor do prompt está em a IA identificar corretamente a lógica das conexões (sequência, paralelismo, agrupamento, continuidade); a sintaxe exata do Mermaid é só o "encanamento" para transformar essa lógica em uma imagem.
