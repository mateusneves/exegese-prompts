# 20. Análise Manuscritológica do Antigo Testamento

**Localização no trabalho:** Seção 4.4 — Análise Manuscritológica

## ⚠️ Seção de alto risco — leia antes de usar

Uma sigla trocada, uma variante "inventada" ou uma data errada são erros graves, difíceis de perceber numa revisão rápida e sérios num trabalho acadêmico. Não existe hoje uma ferramenta gratuita de consulta direta por passagem para o aparato crítico do Antigo Testamento — a BHS e a BHQ são obras com direitos autorais (Deutsche Bibelgesellschaft), só acessíveis via Logos, Accordance, biblioteca ou edição impressa. Por isso, este prompt é rígido quanto à origem dos dados.

## De onde vêm os dados desta seção — três opções

**(a) Aparato crítico copiado do Logos (ou Accordance/BibleWorks/edição impressa) — caminho principal.** Na tela do *Apparatus Criticus* da Biblia Hebraica Stuttgartensia no Logos, copie **somente o trecho referente ao capítulo da sua perícope** e cole no campo indicado no prompt abaixo — evite copiar a página inteira, que geralmente cobre mais de um capítulo/salmo. Como o Logos às vezes inclui capítulos vizinhos mesmo quando você tenta copiar só um, o prompt tem uma regra de segurança para ignorar qualquer entrada que não pertença à sua perícope, caso alguma sobre no recorte.

**(b) Notas textuais de um comentário técnico carregado no notebook**: se algum comentário carregado (ex.: Word Biblical Commentary, NICOT) discute variantes textuais da sua perícope em suas próprias notas, a IA pode se basear nisso, citando o comentarista como fonte — sem fingir ter consultado a BHS/BHQ diretamente.

**(c) Você mesmo monta a comparação com fontes antigas gratuitas**, colando diretamente o texto da mesma passagem em cada versão relevante que você conseguir localizar (nem toda perícope terá todas disponíveis, e a numeração de versículo pode variar entre versões):
- **Septuaginta (grego)** — edição de Rahlfs (1935, domínio público): teste o texto grego do AT já disponível no próprio STEP Bible (stepbible.org) ou em academic-bible.com (Deutsche Bibelgesellschaft).
- **Peshita (siríaco)** — dukhrana.com costuma ter texto siríaco pesquisável; confirme se cobre o livro desejado antes de depender dele.
- **Targum (aramaico)** — sefaria.org tem Targum Onkelos (Torá) e Targum Jônatas (Profetas) com tradução, de graça.
- **Vulgata (latim)** — a Vulgata Clementina (domínio público) está disponível em diversos sites gratuitos.
- **Rolos do Mar Morto (Qumran)** — Leon Levy Dead Sea Scrolls Digital Library (deadseascrolls.org.il): imagens e transcrições gratuitas, mas cobertura limitada aos fragmentos sobreviventes.

Se você não tiver nenhuma das três coisas para esta perícope específica, é mais honesto pular ou simplificar bastante esta seção do que arriscar dados fabricados.

A legenda completa de símbolos e abreviaturas da BHS está dentro do bloco do prompt abaixo (assim ela viaja junto quando você copiar e colar). Ela é baseada em Edson de Faria Francisco, *Principais Símbolos e Abreviaturas do Aparato Crítico da Biblia Hebraica Stuttgartensia* (2008) — carregue este documento como fonte fixa do notebook, além do já recomendado Tov, já que ele cobre siglas raras não listadas na legenda resumida.

## Fontes recomendadas para esta seção
Emanuel Tov, *Textual Criticism of the Hebrew Bible* (critérios de avaliação da crítica textual do Antigo Testamento); Edson de Faria Francisco, *Principais Símbolos e Abreviaturas do Aparato Crítico da BHS* (legenda de siglas); e pelo menos uma das três opções de dados de variantes descritas acima.

## Prompt (copie e cole no NotebookLM)

```text
Com base **exclusivamente** nos dados fornecidos abaixo e nas fontes carregadas neste notebook, redija a seção **"Análise Manuscritológica"** de um trabalho de exegese sobre a perícope **[PASSAGEM]**, texto em hebraico.

Texto da perícope no idioma original (cole aqui, versículo por versículo):
[TEXTO NO IDIOMA ORIGINAL]

Dados sobre variantes textuais desta perícope — cole AO MENOS UMA das três opções abaixo:
(a) Trecho do *Apparatus Criticus* da BHS copiado do Logos (ou de outra edição/software) — copie somente o capítulo da sua perícope:
[TRECHO DO APPARATUS CRITICUS COPIADO DO LOGOS — se disponível]
Dados de citação da edição consultada (autor(es)/editor(es), edição, cidade, editora, ano, página — geralmente o próprio Logos gera essa linha junto com o aparato, cole-a aqui):
[CITAÇÃO DA EDIÇÃO — se disponível]
(b) Notas textuais de comentários carregados neste notebook que discutem variantes desta perícope — identifique aqui quais:
[COMENTÁRIOS COM NOTAS TEXTUAIS SOBRE ESTA PERÍCOPE — se aplicável]
(c) Texto da mesma passagem em versões antigas que você localizou por conta própria (Septuaginta, Peshita, Targum, Vulgata, Qumran) — cole o texto de cada versão que encontrar, identificando qual é qual:
[TEXTO EM VERSÕES ANTIGAS — se aplicável]

Legenda de símbolos e abreviaturas da BHS (use para interpretar as siglas, sem adivinhar nenhuma):
- 𝔐 = Texto Massorético (texto-base); L = Códice de Leningrado B19a (manuscrito-base da BHS, 1008 d.C.); C = Códice do Cairo dos Profetas (895 d.C.).
- 𝔊 = Septuaginta (séc. III-II a.C.); 𝔖 = Peshita (versão siríaca, séc. I-II d.C.); 𝔗 = Targum (paráfrase aramaica); 𝔙 = Vulgata (fim do séc. IV-início do séc. V d.C.); 𝔔 = manuscritos de Qumran (seguido de letra/número do rolo, ex.: 𝔔ᵃ).
- α´ = Áquila; σ´ = Símaco; θ´ = Teodocião; ε´ = Quinta (traduções gregas menores, colunas da Héxapla de Orígenes, séc. II d.C.).
- Ms/Mss = manuscrito(s) hebraico(s) medieval(is) citado(s) nas edições de Kennicott/de Rossi/Ginsburg (não são testemunhas antigas). Quantificadores: `pc Mss` = poucos (3-10); `nonn Mss` = vários (11-20); `mlt Mss` = muitos (21-60); `permlt Mss` = muitíssimos (mais de 60).
- K = ketiv (texto como escrito); Q = qerê (forma indicada para leitura pela tradição massorética).
- Vrs = "muitas ou todas as versões" (menção coletiva, sem especificar qual).
- Termos e sinais críticos: `l`/`leg` = leia-se/lê; `c` = com o apoio de; `cf` = compare; `ad` = para, junto a; `add` = adição; `al` = outros; `dl` = apague; `ins` = insira; `om` = omite; `pr` = antepõe; `tr` = transponha; `var` = leitura variante; `vid` = parece; `m cs` = por razão métrica; `marg` = na margem; `v`/`vv` = verso/versos; `+` = adição; `>` = omissão.
- Marcadores de CONJECTURA do editor (ver regra abaixo): `prb` = provavelmente; `prp` = proposto; `frt` = possivelmente; `*` = conjectura/suposição explícita; `crrp` = corrompido; `dttg`/`homark`/`homtel`/`hpgr` = tipos de erro de cópia hipotetizado (ditografia, homoioarcton, homoioteleuton, haplografia) — todos são juízos críticos do editor, não leituras testemunhadas por manuscrito.

Regras inegociáveis:
- Use somente as entradas do aparato que correspondem exatamente à referência de [PASSAGEM]. Se o trecho colado contiver, ainda assim, alguma entrada de outro capítulo/salmo, ignore-a completamente — não a mencione nem a analise.
- Distinga sempre CONJECTURA de TESTEMUNHO REAL. Se uma nota do aparato usar `prb`, `prp`, `frt` ou `*` SEM nenhuma sigla de manuscrito, versão ou testemunha (𝔊, 𝔖, 𝔗, 𝔙, 𝔔, Ms/Mss, K, Q, α´, σ´, θ´) explicitamente citada ao lado, trate-a como conjectura do editor da BHS, não como variante testemunhada.
- Só use manuscritos, versões e leituras que aparecem explicitamente nos dados colados ou nas fontes carregadas que discutem esta perícope. Não complete com conhecimento geral de crítica textual, não estime datas fora da tabela de referência abaixo ou dos dados fornecidos.
- Quando uma leitura do aparato vier abreviada (terminada em `׳`), verifique se ela corresponde a uma palavra reconhecível no texto no idioma original fornecido acima. Se corresponder, indique a forma completa e a correspondência; só escreva "não determinado nesta fonte" se a abreviação não puder ser conectada a nenhuma palavra do texto fornecido.

Estrutura obrigatória da seção (siga este padrão, usado no modelo de referência):

1. Um parágrafo introdutório citando a origem dos dados e listando em quais versículos da perícope há variantes — mencionando explicitamente quando um versículo não tiver nenhuma.

2. Para cada variante identificada, nesta ordem:
   a. Uma linha de cabeçalho compacta reproduzindo a notação do aparato para aquela unidade (ex.: "Is 1.11a -> 𝔊", "Sl 123.4c - frt dupl (...)").
   b. SE a unidade for uma conjectura pura do editor (sem testemunha citada), não monte tabela — resuma em uma frase no parágrafo de discussão (ex.: "o aparato registra, no v. 3, uma conjectura do editor para suprimir uma palavra por razões métricas, sem apoio de nenhum manuscrito ou versão").
   c. SE houver testemunho real (manuscrito, versão, ou variação massorética Ketiv-Qere), monte uma tabela com as colunas Símbolo | Nome | Data aproximada | Conteúdo da leitura — uma linha por testemunho. Preencha "Nome" e "Data aproximada" com base na legenda e na tabela de referência; se o testemunho específico não estiver identificável (ex.: um Ms sem número, um rolo de Qumran sem sigla completa), escreva "não determinado nesta fonte". Inclua também uma linha para 𝔐 (a leitura do texto-base), identificada na coluna "Nome" como "leitura-base do Texto Massorético — referência de comparação, não é uma variante", para que o leitor veja de imediato o que está sendo contrastado — EXCETO quando a unidade for uma variação Ketiv-Qere (K/Q): nesse caso, a linha do Ketiv já representa a leitura-base impressa, então não inclua uma linha 𝔐 separada, para não duplicar a mesma informação.
   d. Um parágrafo curto discutindo a unidade inteira: testemunho externo (peso e natureza dos testemunhos envolvidos) e testemunho interno (qual leitura explica melhor o surgimento das demais), dialogando quando possível com a obra de crítica textual carregada (ex. Tov) e com comentaristas. Conclua se há impacto relevante sobre a interpretação, a teologia ou a tradução da perícope, ou se é diferença menor.

3. Um parágrafo final de síntese avaliando o grau de estabilidade textual da perícope como um todo, distinguindo quantas variantes tinham testemunho real e quantas eram apenas conjecturas do editor.

Tabela de referência de testemunhos do Antigo Testamento (use SOMENTE estes valores; se não constar aqui, não infira nome nem data):

| Símbolo | Nome | Data aproximada |
|---|---|---|
| 𝔐 | Texto Massorético (texto-base) | Fixado pelos masoretas, séc. VII-X d.C.; testemunha tradição consonantal mais antiga |
| L | Códice de Leningrado B19a (manuscrito-base da BHS) | 1008 d.C. |
| C | Códice do Cairo dos Profetas | 895 d.C. |
| 𝔊 | Septuaginta | Séc. III-II a.C. |
| 𝔖 | Peshita (versão siríaca) | Séc. I-II d.C. |
| 𝔗 | Targum (paráfrase aramaica) | Varia por Targum; geralmente séc. I-V d.C. na forma escrita |
| 𝔙 | Vulgata (versão latina de Jerônimo) | Fim do séc. IV-início do séc. V d.C. |
| 𝔔 | Manuscritos de Qumran | Aprox. séc. III a.C.-I d.C.; use a data do rolo específico se fornecida |
| α´ | Áquila (tradução grega) | Início do séc. II d.C. |
| σ´ | Símaco (tradução grega) | Fim do séc. II d.C. |
| θ´ | Teodocião (tradução grega) | Séc. II d.C. (datação debatida) |
| Ms/Mss | Manuscrito(s) hebraico(s) medieval(is) (Kennicott/de Rossi/Ginsburg) | Período medieval (não são testemunhas antigas) |
| K / Q | Ketiv / Qerê (tradição massorética) | Fixado pelos masoretas, séc. VII-X d.C. |

Requisitos de formato:
- As tabelas devem estar em formato Markdown simples (para copiar depois para o Word).
- Redija os parágrafos de discussão e síntese em prosa acadêmica corrida, em português, terceira pessoa, com citações em nota de rodapé ABNT. Monte a nota completa (SOBRENOME, Nome; ... Título em negrito. Edição. Cidade: Editora, Ano, p. XX) a partir dos dados de citação fornecidos acima (opção a) ou do comentário citado (opção b) — não use uma citação genérica ou incompleta se os dados completos foram fornecidos.
- Se nem aparato, nem comentário, nem versões antigas estiverem disponíveis para esta perícope, diga isso explicitamente e não prossiga com a análise de variantes.
```

## Observações
Depois de gerar o resultado, confira manualmente cada sigla, cada data e cada leitura mencionada contra a fonte original que você colou — não contra a "memória" da IA. Se notar qualquer variante, data ou testemunho que não esteja no que você forneceu, é sinal de que a IA extrapolou e o trecho deve ser removido ou reescrito manualmente. Testado com o Salmo 123 (aparato do Logos): funcionou bem depois de adicionar as regras de filtragem por capítulo e de distinção entre conjectura e testemunho real — se sua perícope tiver notas parecidas com "prb", "prp" ou "frt" sem sigla de testemunha junto, é esperado que a IA as trate como conjectura, não como variante.
