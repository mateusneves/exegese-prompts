# 19. Análise Manuscritológica do Novo Testamento

## MODO DE USO — escolha conforme sua IA:
(A) Se sua IA tem navegação web ativada (Claude com busca, ChatGPT com browsing): ela pode acessar a URL abaixo diretamente.
(B) Se for NotebookLM (sem navegação ao vivo): antes de rodar este prompt, adicione a URL abaixo como fonte ("Adicionar fonte" > "Site"), substituindo a referência pela sua perícope.
(C) Exemplo de URL: https://www.stepbible.org/?q=version=VarApp@version=THGNT@reference=jo.3.1-4&options=GNHVU&pos=1

## Prompt (copie e cole no ChatGPT ou Claude)

```text
URL: https://www.stepbible.org/?q=version=VarApp@version=THGNT@reference=[LIVRO].[CAPÍTULO].[VERSÍCULO-INICIAL]-[VERSÍCULO-FINAL]&options=GNHVU&pos=1


Acesse (ou use como fonte carregada) a URL do StepBible acima, referente à perícope [PASSAGEM]. Extraia os dados do módulo VarApp (Aparato de Variantes Manuscritas do NT) mostrados para cada versículo dessa perícope, e use-os como base EXCLUSIVA para a seção "Análise Manuscritológica".

Legenda do aparato (use para interpretar as siglas, sem adivinhar nenhuma):
- Papiros: "p" + número (p66, p75).
- Unciais: א (aleph), letras maiúsculas latinas/gregas (A, B, C, D, K, L, N, W, Δ, Θ, Ψ), ou número começado em zero (050, 083, 063).
- Famílias de minúsculos: f1, f13.
- Minúsculos individuais: números normais (33, 565, 700, 892...).
- Lecionários: "l" + número; "Lect" = maioria dos lecionários.
- Byz = maioria dos manuscritos bizantinos; Byz2005 = edição Robinson-Pierpont 2005.
- Versões antigas (testemunho de tradução, não manuscrito grego original, mas ainda testemunho externo legítimo): it = latim antigo (itaur, itb, itc...), vg = Vulgata, syr = siríaco (syrc, syrs, syrp, syrh), cop = cóptico (copsa, copbo), arm = armênio, geo = georgiano, got = gótico, slav = eslavo.
- Pais da Igreja: nomes próprios (Orígenes, Tertuliano, Crisóstomo, Agostinho, Cirilo, etc.) — citação do texto por um autor cristão antigo.
- Edições (não são manuscritos, são escolhas editoriais modernas): ς = Textus Receptus; WH = Westcott-Hort; NA = Nestle-Aland (citado só quando difere do texto-base); ECM = Editio Critica Maior.
- Símbolos auxiliares: * após uma sigla = mão original do escriba; número sobrescrito (ex.: א²) ou "c"/"corr" = mão de um corretor posterior; "vid" = leitura provável, mas manuscrito danificado/ilegível nesse ponto; "pc" = pauci (poucos manuscritos adicionais não listados); "pm" = permulti (muitos manuscritos adicionais não listados); "al" = alii (outros manuscritos); "pt" (ex. Byzpt) = só parte daquele grupo testemunha a leitura; "mg" = leitura de margem daquela edição/versão.

IGNORE COMPLETAMENTE as seguintes siglas — são traduções italianas modernas, não são testemunho manuscrito nem edição crítica, e NUNCA devem ser citadas como evidência textual: NR, CEI, ND, Riv, Dio, TILC, Nv, NM.

Regra inegociável: só use manuscritos, versões, Pais da Igreja e edições que aparecem explicitamente nos dados extraídos da URL para esta perícope. Não complete com conhecimento geral de crítica textual, não estime datas de manuscritos que não estejam explícitas nesta fonte, na tabela de referência abaixo, ou nas obras de crítica textual carregadas no notebook.

Estrutura obrigatória da seção (siga este padrão, usado no modelo de referência):

1. Um parágrafo introdutório citando a fonte (StepBible VarApp) e listando em quais versículos da perícope há variantes — e mencionando explicitamente quando um versículo não tiver nenhuma variante registrada.

Antes de detalhar qualquer unidade de variante, verifique se PELO MENOS UMA das leituras tem testemunho manuscrito real — um papiro, um uncial (nomeado ou não), uma família de minúsculos, um minúsculo individual, um lecionário, uma versão antiga ou um Pai da Igreja. Não conta como testemunho manuscrito uma sigla de edição isolada (ς, WH, NA) nem a palavra "Byz" sozinha sem nenhum outro testemunho junto.

Se NENHUMA das leituras de uma unidade tiver testemunho manuscrito real (ou seja, a diferença existir somente entre edições/tradições editoriais modernas), NÃO crie uma seção própria para essa unidade — apenas mencione sua existência, en passant, no parágrafo introdutório (ex.: "há ainda, em João 3.2, duas diferenças que opõem apenas escolhas editoriais — WH de um lado, a tradição bizantina e o Textus Receptus de outro — sem testemunho manuscrito individualizado nesta fonte, por isso não tratadas em detalhe aqui").

2. Trate cada UNIDADE DE VARIANTE (um ponto do texto com leituras concorrentes) como um único bloco — nunca crie um bloco separado por leitura dentro da mesma unidade. Para cada unidade, nesta ordem:
   a. Uma linha de cabeçalho compacta reproduzindo a notação do aparato, mostrando as leituras concorrentes e seus testemunhos (ex.: "Jo 3.2 - αὐτὸν] WH • τὸν Ἰησοῦν] Byz ς").
   b. Uma tabela — SOMENTE SE houver ao menos um testemunho manuscrito principal em alguma das leituras — com as colunas Símbolo | Nome | Data aproximada | Leitura sustentada. Só entram na tabela papiros (p+número) e unciais com nome tradicional consolidado (ver tabela de referência abaixo). NUNCA inclua ς, WH, NA ou Byz como linha de tabela — não são manuscritos. Resuma todos os demais testemunhos de cada leitura (unciais sem nome tradicional, famílias de minúsculos, minúsculos individuais, lecionários, a maioria bizantina, e os agregados pm/pc/al) em UMA frase dentro do parágrafo de discussão (ex.: "a leitura é sustentada ainda pela maioria bizantina e por numerosos minúsculos e lecionários posteriores, não enumerados individualmente"). Se, depois de aplicar esse filtro, nenhuma leitura da unidade tiver testemunho manuscrito principal, não monte tabela — resuma tudo em uma frase.
   c. Um parágrafo curto discutindo a unidade inteira (todas as leituras concorrentes juntas): testemunho externo (peso dos manuscritos principais e o resumo dos secundários), testemunho interno (qual leitura explica melhor o surgimento das demais), e conclusão sobre impacto interpretativo. Mencione a escolha das edições (ς, WH, NA) apenas como informação de contexto dentro desse parágrafo, nunca como testemunho.

3. Um parágrafo final de síntese avaliando o grau de estabilidade textual da perícope como um todo, com base somente nas variantes efetivamente identificadas na fonte do StepBible.

Tabela de referência de MANUSCRITOS do Novo Testamento (use SOMENTE estes valores; qualquer outra sigla de manuscrito entra no resumo genérico da letra b, não na tabela):

| Símbolo | Nome tradicional | Data aproximada |
|---|---|---|
| p45 | Papiro Chester Beatty I | Séc. III |
| p46 | Papiro Chester Beatty II | Séc. II-III |
| p47 | Papiro Chester Beatty III | Séc. III |
| p66 | Papiro Bodmer II | Séc. II-III (c. 200) |
| p72 | Papiro Bodmer VII-VIII | Séc. III-IV |
| p75 | Papiro Bodmer XIV-XV | Séc. II-III (c. 175-225) |
| א (01) | Codex Sinaiticus | Séc. IV |
| A (02) | Codex Alexandrinus | Séc. V |
| B (03) | Codex Vaticanus | Séc. IV |
| C (04) | Codex Ephraemi Rescriptus | Séc. V |
| D (05) | Codex Bezae Cantabrigiensis | Séc. V-VI |
| W (032) | Codex Washingtonianus | Séc. IV-V |

(ς, WH, NA e Byz não entram nesta tabela — são edições/tradição editorial, não manuscritos; use-as apenas na linha de cabeçalho e, no máximo, numa frase do parágrafo de discussão.)

Requisitos de formato:
- As tabelas devem estar em formato Markdown simples (para copiar depois para o Word).
- Redija os parágrafos de discussão e síntese em prosa acadêmica corrida, em português, terceira pessoa, com citação em nota de rodapé ABNT referenciando o StepBible como fonte dos dados do aparato (ex.: STEPBIBLE. New Testament Manuscript Variant Apparatus (VarApp). Disponível em: <URL usada>. Acesso em DD mês. AAAA.).
- Se a fonte não carregar dados para algum versículo da perícope, diga isso explicitamente em vez de inventar uma variante.
```