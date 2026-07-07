# Biblioteca de Prompts para Exegese Bíblica

Biblioteca de prompts para auxiliar na produção de um trabalho de exegese bíblica completa, para qualquer passagem das Escrituras, seguindo a estrutura do modelo de referência: **Arthur Profiro da Costa, "Exegese em Isaías 1.10-20"** (Presbitério de Vila Velha, 2020), redigida a partir da metodologia de Gordon Fee (*Manual de Exegese*), Grant Osborne (*A Espiral Hermenêutica*), Steven Lawson (*Instituto para Pregação Expositiva*) e Wilson Paroschi (*Crítica Textual do Novo Testamento*).

Cada arquivo desta pasta é um prompt independente, correspondente a um item do sumário de uma exegese completa. Rodando os prompts na ordem sugerida abaixo, em uma ferramenta de IA com acesso a fontes bibliográficas (ex.: NotebookLM), você obtém o texto de cada seção do trabalho, pronto para revisão e montagem final no Word.

## Como usar

1. **Crie um notebook novo** (um por perícope em estudo) na ferramenta de IA escolhida.
2. **Carregue as fontes**: comece sempre carregando `00-instrucoes-gerais-notebooklm.md` como uma fonte/documento do notebook. Em seguida, carregue os comentários bíblicos, léxicos, teologias, introduções bíblicas, versões da Bíblia e demais obras relevantes ao livro em estudo (veja a seção 7 do documento de instruções gerais para uma lista recomendada).
3. **Preencha os placeholders**: cada prompt usa campos entre colchetes, como `[LIVRO]`, `[PASSAGEM]`, `[LÍNGUA ORIGINAL]`. Substitua-os pelos dados da sua perícope antes de colar o prompt no notebook. A tabela completa de placeholders está na seção 6 de `00-instrucoes-gerais-notebooklm.md`.
4. **Rode os prompts na ordem sugerida** (veja abaixo). Alguns prompts pedem que você cole o resultado de um prompt anterior como contexto adicional — isso está indicado em cada arquivo, no campo "Fontes recomendadas para esta seção".
5. **Revise cada seção gerada** antes de colar no documento final: confira citações (nomes, páginas, anos), vocalização hebraica/acentuação grega, e se a IA não extrapolou além do que as fontes carregadas realmente sustentam.
6. **Monte o trabalho final** no Word (ou editor de sua preferência) seguindo a ordem do sumário abaixo.

## Ordem de uso recomendada

| # | Arquivo | Seção do trabalho |
|---|---|---|
| — | `00-instrucoes-gerais-notebooklm.md` | (carregar antes de tudo, como fonte fixa) |
| 1 | `02-contexto-historico.md` | 3.1 Contexto Histórico (intro) |
| 2 | `03-autor.md` | 3.1.1 Autor |
| 3 | `04-destinatarios.md` | 3.1.2 Destinatários |
| 4 | `05-data.md` | 3.1.3 Data |
| 5 | `06-circunstancias-historicas.md` | 3.1.4 Circunstâncias Históricas |
| 6 | `07-objetivo-do-autor.md` | 3.1.5 Objetivo do Autor |
| 7 | `08-esboco-geral.md` | 3.1.6 Esboço Geral |
| 8 | `09-contexto-remoto.md` | 3.2.1 Contexto Remoto |
| 9 | `10-contexto-imediato.md` | 3.2.2 Contexto Imediato |
| 10 | `11-estrutura-do-contexto.md` | 3.2.3 Estrutura do Contexto |
| 11 | `12-genero-literario.md` | 3.2.4 Gênero Literário |
| 12 | `13-contexto-canonico-antigo-testamento.md` | 3.3.1 Contexto Canônico — AT |
| 13 | `14-contexto-canonico-novo-testamento.md` | 3.3.2 Contexto Canônico — NT |
| 14 | `15-definicao-da-pericope.md` | 4.2 Definição da Perícope |
| 15 | `16-analise-dos-versiculos.md` | 4.3.1 Análise dos Versículos |
| 16 | `17-traducao-literal.md` | 4.3.2 Tradução Literal |
| — | *(manual)* | 4.3.3 Tradução Dinâmica — sem prompt; adapte a tradução literal para uma leitura fluente |
| 17 | `18-analise-das-versoes.md` | 4.3.4 Análise das Versões |
| 18 | `19-analise-manuscritologica-novo-testamento.md` | 4.4 Análise Manuscritológica |
| 19 | `19-analise-manuscritologica-antigo-testamento.md` | 4.4 Análise Manuscritológica |
| 20 | `21-esboco-lingua-original.md` | 4.5.1 Esboço em Hebraico/Grego |
| 21 | `22-esboco-portugues.md` | 4.5.2 Esboço em Português |
| 22 | `23-comentario-exegetico.md` | 4.6 Comentário Exegético |
| 23 | `24-mensagem-epoca-da-escrita.md` | 4.7 Mensagem para a Época da Escrita |
| 24 | `25-mensagem-para-hoje.md` | 5.1 Mensagem para Hoje |
| 25 | `26-implicacoes-teologia-biblica.md` | 5.2.1 Implicações — Teologia Bíblica |
| 26 | `27-implicacoes-teologia-sistematica.md` | 5.2.2 Implicações — Teologia Sistemática |
| 27 | `28-implicacoes-teologia-pastoral.md` | 5.2.3 Implicações — Teologia Pastoral |
| 28 | `29-esboco-do-sermao.md` | 5.3 Esboço do Sermão |
| 29 | `30-conclusao.md` | 6. Conclusão |
| 30 | `01-introducao.md` | 1. Introdução *(gerar por último)* |

**Sem prompt correspondente** (copiar/colar direto da fonte, ou tarefa manual simples): **2. Texto Bíblico** (colar o texto da perícope na versão escolhida), **4.1 Texto Hebraico/Grego** (colar o texto original da BHS/NA28-UBS), **4.3.3 Tradução Dinâmica** (adaptação manual da tradução literal para leitura fluente).

## Estrutura da pasta

```
exegese-prompts/
├── README.md                                    ← este arquivo
├── 00-instrucoes-gerais-notebooklm.md           ← carregar sempre primeiro
├── 01-introducao.md
├── 02-contexto-historico.md
├── 03-autor.md
├── 04-destinatarios.md
├── 05-data.md
├── 06-circunstancias-historicas.md
├── 07-objetivo-do-autor.md
├── 08-esboco-geral.md
├── 09-contexto-remoto.md
├── 10-contexto-imediato.md
├── 11-estrutura-do-contexto.md
├── 12-genero-literario.md
├── 13-contexto-canonico-antigo-testamento.md
├── 14-contexto-canonico-novo-testamento.md
├── 15-definicao-da-pericope.md
├── 16-analise-dos-versiculos.md
├── 17-traducao-literal.md
├── 18-analise-das-versoes.md
├── 19-analise-manuscritologica-novo-testamento.md
├── 20-analise-manuscritologica-antigo-testamento.md
├── 21-esboco-lingua-original.md
├── 22-esboco-portugues.md
├── 23-comentario-exegetico.md
├── 24-mensagem-epoca-da-escrita.md
├── 25-mensagem-para-hoje.md
├── 26-implicacoes-teologia-biblica.md
├── 27-implicacoes-teologia-sistematica.md
├── 28-implicacoes-teologia-pastoral.md
├── 29-esboco-do-sermao.md
└── 30-conclusao.md
```

## Modelo de referência

Toda a profundidade, formato de citação (ABNT em notas de rodapé) e estilo de redação desta biblioteca foram calibrados a partir de:

> COSTA, Arthur Profiro da. **Exegese em Isaías 1.10-20**. Vila Velha: Presbitério de Vila Velha, 2020. (Trabalho apresentado em cumprimento às exigências para a Licenciatura ao Sagrado Ministério.)

E dos seguintes fundamentos metodológicos:

- FEE, Gordon D. *Manual de Exegese* / *Entendes o que Lês?*
- OSBORNE, Grant R. *A Espiral Hermenêutica*.
- LAWSON, Steven J. *Instituto para Pregação Expositiva* (guia de estudo, OnePassion/Ligonier/Fiel).
- PAROSCHI, Wilson. *Crítica Textual do Novo Testamento*.
- Apostilas do curso "Exegese do Novo Testamento 1 — TE20", Prof. Eduardo Nunes dos Santos (Aula 04 — Análise Contextual; Aula 12 — Análise Teológica).

## Limitações e boas práticas

- Estes prompts pressupõem que a IA usada (NotebookLM ou similar) só responde com base nas fontes carregadas no notebook, e não com conhecimento geral irrestrito. Se você migrar para outra ferramenta de IA sem esse tipo de restrição, adicione uma instrução explícita reforçando "responda apenas com base nos documentos anexados" antes de cada prompt.
- Textos gerados por IA sobre línguas originais (hebraico/grego) e aparato crítico exigem revisão humana cuidadosa — erros de caractere, vocalização ou notação são comuns.
- Esta biblioteca não substitui o trabalho intelectual do próprio exegeta: os prompts entregam uma primeira compilação sintetizada das fontes, mas a responsabilidade de revisão crítica, ajuste teológico e redação final é sempre do usuário.
