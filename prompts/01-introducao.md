# 1. Introdução

**Localização no trabalho:** Seção 1 — INTRODUÇÃO
**Quando usar:** Por último, depois de ter gerado todas as demais seções (a introdução resume o método e o percurso do trabalho já concluído).

## O que este prompt gera
O parágrafo (ou conjunto de parágrafos) de abertura do trabalho: apresentação do objetivo da pesquisa, breve nota sobre o problema/tema central da perícope, método utilizado (histórico-gramatical), fontes principais empregadas e um roteiro de como o trabalho está dividido (Estudo Contextual, Estudo Textual, Estudo Teológico).

## Fontes recomendadas para esta seção
Este prompt não depende de fontes externas específicas — ele sintetiza o que já foi produzido nas demais seções. Tenha em mãos (ou cole como contexto) os textos já gerados de Contexto Histórico, Definição da Perícope e Mensagem para Hoje, se possível.

## Prompt (copie e cole no NotebookLM)

"""
Com base exclusivamente nas fontes carregadas neste notebook, redija a seção **"Introdução"** de um trabalho de exegese bíblica sobre a perícope **[PASSAGEM]**, do livro de **[LIVRO]**.

A introdução deve conter, nesta ordem, em prosa corrida (sem subtítulos):

1. Um parágrafo que apresente o objetivo da pesquisa: analisar a perícope [PASSAGEM] considerando seus elementos históricos, gramaticais e teológicos, a fim de obter a mensagem do texto e aplicá-la ao leitor contemporâneo. Inclua uma frase-síntese de uma a duas linhas sobre do que trata o texto (o "problema" ou tema central da perícope), com base no que as fontes disponíveis dizem sobre o assunto.
2. Um parágrafo que declare o método utilizado — histórico-gramatical —, explicando resumidamente o que esse método busca (elementos históricos do período e do autor, o contexto dos destinatários, a forma da escrita e os termos gramaticais utilizados) e cite os tipos de fontes utilizadas na pesquisa (comentários bíblicos, léxicos, bíblias em várias versões, teologias sistemáticas e bíblicas, introduções ao Antigo/Novo Testamento e outras obras), sempre baseando-se nas fontes efetivamente carregadas neste notebook.
3. Um parágrafo final que funcione como roteiro do trabalho, explicando que a pesquisa está dividida em três partes — Estudo Contextual, Estudo Textual e Estudo Teológico — e resumindo em uma frase o que será visto em cada uma dessas partes.

Requisitos de formato:
- Redija em prosa acadêmica corrida, em português, terceira pessoa.
- Cite em nota de rodapé, no padrão ABNT, a fonte usada para a bíblia/versão citada no corpo do texto, se houver referência direta a uma tradução específica.
- Não invente dados que não estejam nas fontes disponíveis; se o método ou o tema central não estiverem explícitos nas fontes, generalize com cautela a partir do que a perícope e o contexto do livro permitem inferir.
- Extensão aproximada: 3 parágrafos.
"""

## Observações
Esta é a única seção que deve ser gerada por último, pois depende do conteúdo das demais. Ao rodar este prompt, cole como contexto adicional (na mesma conversa do NotebookLM) um resumo das seções já produzidas, para que a IA consiga sintetizar com precisão o "roteiro do trabalho".
