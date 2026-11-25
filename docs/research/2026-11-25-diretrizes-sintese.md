# Diretrizes de síntese e verificação: o que PRISMA 2020, Cochrane, JBI e SWiM exigem

| | |
|---|---|
| **Issue** | #3 (`wayfinder:research`) |
| **Data** | 2026-11-25 |
| **Branch** | `research/diretrizes-sintese` |
| **Pergunta** | O que as diretrizes de revisão sistemática exigem de uma **síntese** e da sua **verificação**, para servir de checklist a um app? |

---

## Resposta curta

As quatro fontes convergem em cinco exigências:

1. dizer **como os estudos foram agrupados** (por população, intervenção, desfecho ou desenho);
2. **nomear e justificar o método** de síntese;
3. mostrar **o resultado por desfecho**, com direção e magnitude;
4. tratar **inconsistência e contradições** de forma explícita;
5. avaliar a **certeza da evidência**.

A verificação, portanto, não pergunta "o texto está bem escrito?", e sim: **cada afirmação tem lastro rastreável e cada elo entre estudo → síntese → conclusão está declarado?**

> **Aviso de escopo.** PRISMA 2020 e SWiM são diretrizes de **relato** — dizem o que precisa ser escrito, não como conduzir a revisão. O próprio artigo do SWiM alerta que a diretriz "não deve ser usada para guiar a condução da síntese" nem como instrumento de qualidade. Cochrane e JBI cobrem condução **e** relato. Consequência prática para o app: ele pode checar se a síntese **declara** o que deveria; ele **não** pode prometer julgar se a revisão foi bem conduzida.

### Termos usados neste documento

| Termo | Em linguagem simples |
|---|---|
| **Síntese** | A parte da revisão em que os achados de vários estudos são juntados e interpretados. |
| **Meta-análise** | Síntese estatística que produz um número único (efeito médio) a partir de vários estudos. |
| **Síntese sem meta-análise** | Juntar os resultados sem produzir esse número único — por tabela, direção do efeito, faixa de efeitos etc. |
| **Heterogeneidade** | O quanto os estudos discordam entre si. Medida por Q, I² e Tau². |
| **I²** | Percentual da variação entre estudos que não é fruto do acaso. |
| **IC (intervalo de confiança)** | Faixa em que o valor verdadeiro provavelmente está. |
| **GRADE** | Sistema para dizer o quão confiável é a evidência de um desfecho (alta, moderada, baixa, muito baixa). |
| **ConQual** | Equivalente do GRADE para achados de síntese qualitativa. |
| **SoF** | *Summary of findings*: tabela que resume, por desfecho, efeito, número de estudos e certeza. |

---

## 1. As quatro fontes em uma página

| Fonte | O que cobre | O que acrescenta de único |
|---|---|---|
| **PRISMA 2020** | Relato de revisões sistemáticas. O item 13 é o núcleo da síntese, com seis subitens (13a–13f). Itens 20 a 23 espelham a síntese nos resultados e na discussão. | Estrutura obrigatória de relato, item por item, com numeração estável — a melhor base para um verificador. |
| **Cochrane Handbook v6.5 (2024)** | Condução e relato. Capítulos relevantes: 3, 9, 10, 12, 14 e 15. | Critérios de aceitabilidade dos métodos; o que é explicitamente inaceitável; GRADE e tabelas SoF. |
| **JBI Manual** | Capítulo 3: síntese de evidência **qualitativa** (meta-agregação e ConQual). Capítulo 4: síntese de **efetividade** (meta-análise). | A única das quatro que trata a síntese qualitativa com o mesmo rigor da quantitativa, com vocabulário próprio (achado, categoria, achado sintetizado). |
| **SWiM** | Nove itens de relato para quando **não há meta-análise** de efeitos. | Detalhamento que o PRISMA não oferece: métrica padronizada, priorização de estudos, apresentação ordenada, limitações da própria síntese. |

---

## 2. Exigências por diretriz

### 2.1 PRISMA 2020 — item 13 e correlatos

O item 13 se chama, no original, "Synthesis methods". Ele é dividido em seis subitens. A coluna da direita traduz o que cada um exige na prática.

| Subitem | Exigência (paráfrase) | O que significa na prática |
|---|---|---|
| **5** | Especificar os critérios de inclusão e exclusão **e como os estudos foram agrupados para as sínteses**. | O agrupamento não é detalhe de bastidor: é item de método. |
| **13a** | Descrever o processo usado para decidir **quais estudos eram elegíveis para cada síntese** (por exemplo, tabulando características da intervenção e comparando com os grupos planejados no item 5). | Cada síntese tem seu próprio conjunto de estudos, e isso precisa ser justificado. |
| **13b** | Descrever os métodos de **preparo dos dados** para a síntese — dados faltantes, conversões de dados. | Se houve conversão de medida, o método precisa ser citado. |
| **13c** | Descrever os métodos de **tabulação ou apresentação visual** dos resultados dos estudos individuais e das sínteses. | Tabelas e figuras são método, não enfeite. |
| **13d** | Descrever os métodos de **síntese** e **justificar a escolha**. Se houve meta-análise, descrever modelo, método de heterogeneidade e software. **Se não houve**, descrever como os resultados foram sumarizados (estatísticas-resumo, direção do efeito, combinação de valores de p) e como a heterogeneidade foi explorada. | Este é o item que o SWiM detalha. É o coração da verificação. |
| **13e** | Descrever os métodos usados para **explorar causas de heterogeneidade** (subgrupos, meta-regressão). | Inclui métodos informais, como ordenar tabelas por modificador hipotetizado. |
| **13f** | Descrever as **análises de sensibilidade** feitas para testar a robustez do resultado sintetizado. | "O resultado muda se eu tirar os estudos frágeis?" |

**Itens correlatos que fecham o ciclo:**

| Item | Exigência |
|---|---|
| **15** | Descrever os métodos de avaliação de risco de viés **e de certeza da evidência** para cada desfecho. |
| **20a** | Para cada síntese, resumir as **características e o risco de viés** dos estudos que contribuíram. |
| **20b** | Apresentar os resultados de **todas** as sínteses estatísticas: estimativa sumária e precisão; medidas de heterogeneidade; **direção do efeito**. |
| **20c** | Apresentar os resultados de **todas** as investigações de causas de heterogeneidade. |
| **20d** | Apresentar os resultados de **todas** as análises de sensibilidade. |
| **21** | Apresentar a avaliação de risco de viés **por resultados faltantes** (viés de publicação), para cada síntese. |
| **22** | Apresentar a avaliação de **certeza da evidência para cada desfecho**. |
| **23b, 23c** | Discutir as limitações **da evidência incluída** e as limitações **dos processos da revisão**. São coisas diferentes. |

### 2.2 Cochrane Handbook (v6.5, 2024)

**Capítulo 3 — Definir critérios e agrupar estudos para a síntese.**
O capítulo trata o agrupamento como decisão metodológica de primeira ordem: os critérios de elegibilidade e a forma de agrupar (população, intervenção, comparação, desfecho, desenho) precisam ser definidos antes de ver os resultados, e mudanças posteriores precisam ser justificadas. É a base do item 1a/1b do SWiM.

**Capítulo 9 — Resumir características dos estudos e preparar a síntese.**
Propõe um percurso em etapas: identificar as comparações e desfechos que serão sintetizados; determinar **quais estudos contribuem para cada síntese**; examinar as características de cada estudo; avaliar o risco de viés; e só então decidir se a síntese é apropriada e qual método usar. A mensagem central: **agrupar é uma decisão, e ela precisa ser visível para o leitor.** É também o capítulo que sustenta a checagem de sobreposição — se o mesmo estudo entra em duas sínteses com o mesmo dado, o leitor não tem como saber.

**Capítulo 10 — Analisar dados e realizar meta-análises (heterogeneidade).**
Define os instrumentos: estatística Q, I² e Tau². O Handbook dá faixas de referência para o I² (aproximadamente 0–40% pode não ser importante, 30–60% moderada, 50–90% substancial, 75–100% considerável), mas ressalta que essas faixas não são regra absoluta e que a diversidade clínica e metodológica deve ser examinada **antes** da estatística. Trata também da escolha entre modelo de efeitos fixos e aleatórios.

**Capítulo 12 — Sintetizar e apresentar achados usando outros métodos.**
É o capítulo que o SWiM usa como referência de condução. Pontos que importam para o app:

- Métodos aceitáveis quando não há meta-análise: **sumarizar estimativas de efeito** (mediana, faixa, intervalo interquartil), **combinar valores de p** e **contagem de votos baseada na direção do efeito**.
- **Inaceitável:** contagem de votos baseada em **significância estatística**.
- "Síntese narrativa" sem descrição do método **não é suficiente** — é exatamente a lacuna que o SWiM foi criado para fechar.
- O método escolhido e suas limitações precisam ser declarados, porque **o método determina a pergunta que a síntese responde** (ver item 9 do SWiM).

**Capítulo 14 — Tabelas SoF e GRADE.**
A certeza é avaliada **por desfecho**, não para a revisão inteira. Cinco domínios rebaixam a certeza: risco de viés, inconsistência, indiretividade (o estudo não mede exatamente o que a pergunta pede), imprecisão e viés de publicação. Três domínios podem elevar: magnitude grande do efeito, relação dose-resposta e confundidores plausíveis que reduziriam o efeito observado. A tabela SoF resume, por desfecho, o efeito, o número de participantes e a certeza.

**Capítulo 15 — Interpretar resultados e tirar conclusões.**
Separa o que os dados mostram do que isso significa. Distingue limitações **da evidência** de limitações **da revisão**. E adverte contra o erro clássico: transformar "não encontramos evidência" em "há evidência de que não funciona".

### 2.3 JBI Manual

**Capítulo 3 — Revisões sistemáticas de evidência qualitativa.**

- **3.3.13 (síntese de dados):** o método padrão é a **meta-agregação**. O percurso é: *achados* extraídos dos estudos (cada um classificado quanto à credibilidade — inequívoco, equívoco ou não suportado) → *categorias* → *achados sintetizados*.
- **3.3.13.2 (achados sintetizados):** cada achado sintetizado precisa de um **enunciado explicativo**, precisa estar ligado à pergunta da revisão e **não deve ser redigido como recomendação**. Dados divergentes não devem ser forçados a caber numa categoria única.
- **3.3.15 (ConQual):** a confiança no achado sintetizado é avaliada por dois componentes — **credibilidade** (depende da proporção de achados inequívocos versus equívocos que sustentam o achado) e **dependabilidade** (cinco critérios de qualidade do relato dos estudos primários). O resultado é um nível de confiança, com rebaixamento.

**Capítulo 4 — Revisões sistemáticas de efetividade.**

- **4.4.7.5 (síntese de dados):** exige descrever o objetivo da síntese, a medida de efeito, o modelo (fixo ou aleatório), o método de combinação, os testes e indicadores de heterogeneidade (Q, I²), e as análises de sensibilidade e de subgrupo.

### 2.4 SWiM — os nove itens

O SWiM é uma extensão do PRISMA para revisões de intervenção em que **não** se faz meta-análise de estimativas de efeito. Os nove itens, na tradução de trabalho:

| # | Item | O que exige |
|---|---|---|
| **1a** | Agrupamento dos estudos | Descrição **e justificativa** dos grupos usados na síntese (populações, intervenções, desfechos, desenho). |
| **1b** | Mudanças após o protocolo | Detalhar e justificar qualquer mudança nos grupos depois do protocolo. |
| **2** | Métrica padronizada | Descrever a métrica de cada desfecho, explicar por que foi escolhida e descrever as transformações aplicadas, citando a orientação metodológica consultada. |
| **3** | Métodos de síntese | Descrever e justificar os métodos usados para sintetizar cada desfecho quando não foi possível a meta-análise. |
| **4** | Critérios de priorização | Onde aplicável, dizer com que critério certos estudos foram priorizados na síntese principal ou na conclusão (desenho, risco de viés, relevância). |
| **5** | Heterogeneidade | Declarar os métodos usados para examinar heterogeneidade quando não houve meta-análise, e dizer se a investigação não era pré-especificada. |
| **6** | Certeza da evidência | Descrever os métodos de avaliação da certeza dos achados da síntese. |
| **7** | Apresentação dos dados | Descrever tabelas e gráficos usados, e **especificar as características dos estudos usadas para ordená-los**, referenciando os estudos. |
| **8** | Relato dos resultados | Para cada comparação e desfecho: descrever os achados sintetizados **e a certeza**, em linguagem compatível com a pergunta, indicando **quais estudos contribuem**. |
| **9** | Limitações da síntese | Relatar as limitações dos métodos e dos agrupamentos e **como elas afetam as conclusões** possíveis. |

Dois pontos do artigo que valem para o desenho do app:

- O SWiM traz uma tabela que associa **método → pergunta respondida**. Se a métrica é direção do efeito e o método é contagem de votos, a pergunta é "há alguma evidência de efeito?", não "qual é o efeito médio?". Confundir as duas é erro de interpretação, não de redação.
- O SWiM **complementa** o PRISMA; não o substitui.

---

## 3. O que é comum às quatro (o núcleo irredutível)

| Elemento da síntese | PRISMA | Cochrane | JBI | SWiM |
|---|---|---|---|---|
| Agrupamento declarado | 5, 13a | cap. 3 | 3.3.13 | 1a, 1b |
| Métrica e transformações | 13b | cap. 6 | 4.4.7.5 | 2 |
| Método nomeado e justificado | 13d | cap. 12 | 3.3.13 / 4.4.7.5 | 3 |
| Critério de priorização | 13a | cap. 9 | — | 4 |
| Heterogeneidade / inconsistência | 13e | cap. 10 | 4.4.7.5 | 5 |
| Contradições e dados divergentes | 13e, 20c | cap. 9, 15 | 3.3.13, 3.3.15 | 8 |
| Certeza por desfecho | 15, 22 | cap. 14 | 3.3.15 (ConQual) | 6 |
| Apresentação ordenada | 13c | cap. 12 | 3.3.13.2 | 7 |
| Resultado com direção e magnitude | 20b | cap. 12, 15 | 3.3.13.2 | 8 |
| Lastro estudo → afirmação | 20a, 20b | cap. 9 | 3.3.13.2 | 8 |
| Limitações da síntese | 23c | cap. 15 | — | 9 |

Onde as quatro **não** convergem: só o JBI tem um sistema próprio de confiança para achados qualitativos (ConQual); só o SWiM tem item específico para "mudanças após o protocolo"; e só o PRISMA numera, de forma estável, os itens de relato.

---

## 4. Checklist acionável (12 itens)

**Como usar:** os itens 1 a 5 são **por revisão** (uma vez). Os itens 6 a 12 são **por desfecho ou comparação** (repetem). "Crítico" significa que a ausência impede a verificação; "Alerta" significa que a síntese existe, mas o leitor não consegue julgar a robustez.

| # | O que verificar | Como o app verifica | Se faltar | Fonte |
|---|---|---|---|---|
| **1** | A pergunta e o **agrupamento** dos estudos estão declarados. | Procurar, na seção de métodos, a frase que diz como os estudos foram agrupados. Conferir se cada desfecho da pergunta aparece em algum grupo. | Crítico | PRISMA 5, 13a; Cochrane 3; SWiM 1a |
| **2** | Existe **critério explícito** para decidir quais estudos entram em cada síntese. | Procurar frase de priorização (desenho, risco de viés, relevância). Se não houver, verificar se todos os estudos elegíveis entram em todas as sínteses. | Alerta | SWiM 4; PRISMA 13a |
| **3** | A **métrica** está nomeada e as **transformações** descritas. | Identificar a unidade do resultado (RR, OR, MD, SMD, direção, p). Se houve conversão, exigir citação do método. | Crítico | PRISMA 13b; SWiM 2 |
| **4** | O **método de síntese** está nomeado, justificado e é compatível com a pergunta. | Se a pergunta é "qual o efeito médio", exigir meta-análise ou estatísticas-resumo; se é "há evidência em algum estudo", admitir combinação de p; se é "há alguma evidência", admitir contagem por direção. | Crítico | PRISMA 13d; Cochrane 12; SWiM 3; JBI 4.4.7.5 |
| **5** | A **inconsistência** foi examinada e relatada. | Procurar I², Tau², Q ou descrição de inspeção ordenada. Se não houve, exigir justificativa. | Alerta | PRISMA 13e; Cochrane 10; SWiM 5; JBI 4.4.7.5 |
| **6** | Para cada desfecho: **direção**, **magnitude**, **número de estudos e participantes** e **IC** quando possível. | Conferir se cada desfecho da lista traz os quatro dados. IC ausente exige justificativa. | Crítico | PRISMA 20b; SWiM 8 |
| **7** | Tabelas e figuras estão **ordenadas como o texto** e trazem desenho e risco de viés. | Comparar a ordem da tabela com a ordem dos parágrafos; verificar se as colunas obrigatórias existem. | Alerta | PRISMA 13c; SWiM 7 |
| **8** | **Contradições e dados divergentes** são mencionados, não diluídos. | Procurar estudos com efeito oposto. Se todos os achados aparecem como concordantes, suspeitar de omissão. | Crítico | JBI 3.3.13, 3.3.15; Cochrane 9, 15 |
| **9** | A **certeza da evidência** é dada por desfecho, com método e motivo do rebaixamento. | Procurar tabela SoF ou frase por desfecho. "Alta/moderada/baixa" sem justificativa é relato incompleto. | Crítico | PRISMA 15, 22; Cochrane 14; SWiM 6; JBI 3.3.15 |
| **10** | Cada afirmação da síntese **aponta para os estudos** que a sustentam. | Para cada frase de resultado, exigir referência a estudos (no texto ou em tabela). Frase sem nenhuma referência = afirmação órfã. | Crítico | SWiM 8; JBI 3.3.13.2; Cochrane 9 |
| **11** | As **limitações da síntese** (métrica, método, agrupamento) e o que elas impedem de concluir. | Procurar seção de limitações que fale do **método**, não só dos estudos incluídos. | Crítico | PRISMA 23c; SWiM 9; Cochrane 15 |
| **12** | **Sensibilidade** e **viés de publicação** foram avaliados. | Procurar análise de sensibilidade e avaliação de viés de publicação (gráfico de funil, Egger) ou justificativa de impossibilidade. | Alerta | PRISMA 13f, 20d, 21 |

---

## 5. Como o verificador decide (e o que ele não decide)

### 5.1 Três níveis de resultado

| Nível | Condição | Efeito no app |
|---|---|---|
| **Reprovado** | Falta o item **4**, **6**, **10** ou **11**. | Bloqueia a publicação do resumo. Sem método nomeado, sem resultado por desfecho, sem lastro ou sem limitações declaradas, não há síntese verificável — há opinião. |
| **Alerta** | Falta o item **2**, **5**, **7** ou **12**. | Permite publicar, mas exibe ressalva explícita. |
| **Aprovado** | Todos os itens de 1 a 12 presentes — ou ausência apenas entre os itens 2, 5, 7 e 12, com justificativa registrada. | Publica com o quadro de conformidade. |

> Estas três faixas são uma **proposta de regra do app**, não uma classificação prevista nas diretrizes. Nenhuma das quatro fontes define "aprovado/reprovado". O app deve dizer isso ao usuário.

### 5.2 O que o verificador **não** pode fazer

- **Não julgar se o método escolhido é o melhor.** Ele julga se o método foi declarado e se a conclusão respeita o que aquele método permite concluir (SWiM, item 9).
- **Não avaliar qualidade da revisão.** PRISMA e SWiM são de relato; usá-los como nota de qualidade é aplicação indevida, alertada no próprio artigo do SWiM.
- **Não substituir o julgamento humano** sobre risco de viés ou certeza. Ele pode checar se a avaliação existe e se está justificada; não pode refazê-la.

### 5.3 Checagens de sobreposição e repetição

O item 10 (lastro) não basta sozinho. Três verificações adicionais, derivadas de PRISMA 20a e Cochrane cap. 9:

1. **Dupla contagem:** o mesmo estudo aparece em duas sínteses com o mesmo desfecho e os mesmos participantes? Sinal de que o dado foi contado duas vezes.
2. **Sobreposição de afirmações:** a mesma conclusão aparece em duas seções com palavras diferentes? Sinal de inflação artificial do número de achados.
3. **Achado sintetizado sem estudo de origem:** no caso qualitativo, um achado sintetizado que não remete a nenhuma categoria nem a nenhum achado primário viola o percurso do JBI 3.3.13.

---

## 6. Riscos de IA generativa nesta etapa

O que segue não é opinião: cada risco tem fonte e cada recomendação tem lastro. A regra institucional mais importante está no fim desta seção.

### 6.1 Referência inventada (alucinação bibliográfica)

**O que a literatura mostra.** Walters e Wilder avaliaram 636 citações produzidas por ChatGPT em 84 textos. **55% das citações do GPT-3.5 e 18% das do GPT-4 eram fabricadas** — não correspondiam a obras reais. Entre as citações que apontavam para obras reais, **43% (GPT-3.5) e 24% (GPT-4) tinham erros substantivos** (autoria, título, revista, volume, páginas, ano). O estudo também registra que os modelos frequentemente **confirmam** a validade de uma citação falsa quando questionados.

**Por que acontece.** Um modelo de linguagem prevê a próxima palavra; ele não consulta uma base bibliográfica. A citação é gerada como texto plausível, não como registro recuperado.

**Recomendação para o app.**
- Nunca aceitar referência sem identificador verificável (DOI ou PMID) conferido em base primária.
- Exibir um selo "verificado / não verificado" por referência, e não permitir exportar bibliografia com item não verificado.
- Manter o humano como autor da lista de referências: a IA pode sugerir, não decidir.

### 6.2 Perda de nuance na síntese qualitativa

**O que a literatura mostra.** Pizard e colegas, em dois experimentos com síntese qualitativa assistida por LLM, relatam: temas **genéricos e superficiais**; falha em reproduzir decisões reflexivas da síntese manual (por exemplo, criar uma categoria nova no meio do processo); e um risco que chamam de "confundir forma com conteúdo" — o texto parece útil à primeira vista e se revela inconsistente no exame detalhado. Castellanos e colegas compararam temas gerados por LLM com temas de codificadores humanos em 310 tópicos: houve **79,7% de concordância**, mas o modelo classificou como coerentes **96% dos tópicos que os humanos julgaram de baixa coerência**, e tratou subtemas divergentes como convergentes.

**Tradução.** O modelo tende a **suavizar o que é conflitante** e a produzir coerência onde os dados não a sustentam. É o oposto do que JBI 3.3.13.2 exige (dados divergentes não devem ser forçados).

**Recomendação para o app.**
- No fluxo qualitativo, exigir a cadeia auditável **achado → categoria → achado sintetizado**, com o estudo de origem em cada elo.
- Nunca deixar a IA redigir o enunciado explicativo sem checagem humana registrada.
- Sinalizar automaticamente textos em que **todos** os achados são apresentados como concordantes — pode ser perda de nuance, não consenso.

### 6.3 Viés de agregação

O termo tem dois sentidos, e os dois importam.

**(a) Agregação estatística indevida.** Juntar estudos heterogêneos produz um número médio que responde a uma pergunta que ninguém fez (Cochrane cap. 10). O SWiM item 9 exige declarar exatamente isso: a escolha de métrica e método **define a pergunta** que a síntese responde.

**(b) Agregação cognitiva da IA.** Castellanos documenta supergeneralização e "overfitting" temático — o modelo força coerência a partir de um único post. Pizard registra viés de população WEIRD (ocidental, escolarizada, industrializada, rica e democrática) nos modelos e dificuldade de representar outros contextos.

**Recomendação para o app.**
- Exibir, em cada síntese, **a pergunta que aquele método realmente responde** (lógica da tabela 2 do SWiM).
- Alertar quando o método mudou em relação ao protocolo e a mudança não foi justificada (SWiM 1b).
- Em revisões com populações não WEIRD, registrar explicitamente o risco de viés de contexto.

### 6.4 Reprodutibilidade e caixa-preta

**O que a literatura mostra.** Pizard observa que a decodificação por amostragem faz o mesmo prompt gerar respostas diferentes, e que fornecedores alteram modelos sem avisar. A declaração conjunta Cochrane–Campbell–JBI–CEE exige registrar **nome, versão e data** da ferramenta, a finalidade, a justificativa e as limitações.

**Recomendação para o app.**
- Registrar prompt, modelo, versão, data e saída de cada geração, e não sobrescrever esse log.
- Não regenerar texto silenciosamente: toda nova versão deve ficar rastreável.

### 6.5 Responsabilidade, supervisão humana e transparência

A **Declaração de posição de 2025** de Cochrane, Campbell, JBI e CEE (baseada nas recomendações RAISE) é a referência institucional mais direta para o app. Os pontos que importam:

- O autor é **responsável final** pelo conteúdo, pelos métodos e pelos achados, inclusive pela decisão de usar IA.
- IA pode ser usada **desde que se demonstre** que não compromete o rigor metodológico nem a integridade da síntese.
- Uso de IA **com supervisão humana**.
- Qualquer uso que **faça ou sugira julgamentos** deve ser declarado de forma transparente. A lista inclui explicitamente: elegibilidade de estudo, avaliação de risco de viés, extração de dados, **síntese de dados de dois ou mais estudos** e **avaliação da certeza da evidência**.
- A justificativa precisa incluir evidência de que a ferramenta é metodologicamente sólida e foi validada no contexto daquela síntese.

**Recomendação para o app.**
- Separar visualmente o que foi **decisão humana** e o que foi **sugestão da IA**.
- Gerar automaticamente o parágrafo de declaração de uso de IA, no formato sugerido pela declaração.
- Não se apresentar como ferramenta clínica validada, nem como substituto do julgamento do revisor.

### 6.6 Panorama: a IA já é confiável para sintetizar?

A revisão de escopo de Lieberum e colegas mapeou 37 artigos sobre LLMs em revisões sistemáticas. Os modelos foram aplicados em 10 das 13 etapas do processo, mais frequentemente busca (41%), seleção de estudos (38%) e extração de dados (30%). Os autores avaliaram o uso como promissor em 54% dos estudos, neutro em 24% e **não promissor em 22%**. A conclusão dos autores: **faltam aplicações plenamente estabelecidas ou validadas** — o título do artigo é "on the rise, but not yet ready for use" (em ascensão, mas ainda não prontas para uso).

Isso não impede usar IA como apoio. Impõe que o app trate toda saída como **rascunho a verificar**, não como resultado.

### 6.7 Quadro-resumo: risco → sinal → regra

| Risco | Como aparece no texto | Regra do app |
|---|---|---|
| Citação inventada | Referência sem DOI/PMID, ou com dados que não batem | Bloquear exportação até verificação |
| Perda de nuance | Todos os achados concordantes; temas amplos e genéricos | Exigir cadeia achado → categoria → achado sintetizado |
| Coerência forçada | Subtemas divergentes tratados como convergentes | Checar cada subtema contra o estudo de origem |
| Viés de agregação | Efeito médio calculado sobre estudos heterogêneos | Mostrar a pergunta que o método responde |
| Perda de contexto | Síntese ignora população, cenário ou país | Exigir característica de contexto por estudo |
| Irreprodutibilidade | Sem registro de modelo/versão/prompt | Log imutável por geração |
| Responsabilidade difusa | Texto não distingue decisão humana de sugestão | Marcação por origem + declaração automática |

---

## 7. Limitações desta pesquisa

- **Não é uma revisão sistemática.** Foi uma consulta dirigida às fontes primárias citadas, não uma busca exaustiva com protocolo.
- **Cochrane é documento vivo.** A versão consultada é a 6.5 (2024); a numeração de capítulos e seções pode mudar em versões futuras.
- **JBI é wiki atualizada continuamente.** Os números de seção (3.3.13, 3.3.13.2, 3.3.15, 4.4.7.5) refletem o estado do Manual no momento da consulta.
- **Acesso ao texto completo.** O PRISMA 2020 e o SWiM foram lidos na versão PMC, porque o site do BMJ bloqueou acesso direto. O conteúdo é o mesmo artigo, em acesso aberto.
- **Literatura de IA muda rápido.** As evidências sobre desempenho de LLMs datam de 2023–2025 e devem ser rechecadas antes de cada versão do app. O estudo de Pizard é **preprint** (arXiv), ainda sem revisão por pares — foi usado apenas para riscos qualitativos, com apoio do estudo revisado de Castellanos.
- **Escopo deliberadamente restrito** às quatro fontes pedidas na Issue. GRADE-CERQual, AMSTAR 2 e ROBIS ficaram de fora.

---

## 8. Fontes

### Diretrizes

- **PRISMA 2020** — Page MJ, McKenzie JE, Bossuyt PM, et al. *The PRISMA 2020 statement: an updated guideline for reporting systematic reviews.* BMJ 2021;372:n71. DOI: [10.1136/bmj.n71](https://doi.org/10.1136/bmj.n71). Texto completo em acesso aberto: [PMC8005924](https://pmc.ncbi.nlm.nih.gov/articles/PMC8005924/). Checklist oficial: [prisma-statement.org](http://www.prisma-statement.org/).
- **Cochrane Handbook for Systematic Reviews of Interventions**, versão 6.5 (2024). Capítulos consultados: [3](https://training.cochrane.org/handbook/current/chapter-03), [9](https://training.cochrane.org/handbook/current/chapter-09), [10](https://training.cochrane.org/handbook/current/chapter-10), [12](https://training.cochrane.org/handbook/current/chapter-12), [14](https://training.cochrane.org/handbook/current/chapter-14), [15](https://training.cochrane.org/handbook/current/chapter-15).
- **JBI Manual for Evidence Synthesis.** [Manual completo](https://jbi-global-wiki.refined.site/space/MANUAL). Seções consultadas: [3.3.13 — Data synthesis](https://jbi-global-wiki.refined.site/space/MANUAL/863863028), [3.3.13.2 — Synthesised findings](https://jbi-global-wiki.refined.site/space/MANUAL/863863040), [3.3.15 — ConQual](https://jbi-global-wiki.refined.site/space/MANUAL/864551003), [4.4.7.5 — Data synthesis (efetividade)](https://jbi-global-wiki.refined.site/space/MANUAL/355828857).
- **SWiM** — Campbell M, McKenzie JE, Sowden A, et al. *Synthesis without meta-analysis (SWiM) in systematic reviews: reporting guideline.* BMJ 2020;368:l6890. DOI: [10.1136/bmj.l6890](https://doi.org/10.1136/bmj.l6890). Texto completo: [PMC7190266](https://pmc.ncbi.nlm.nih.gov/articles/PMC7190266/). Site do projeto: [swim.sphsu.gla.ac.uk](https://swim.sphsu.gla.ac.uk).

### Inteligência artificial na síntese

- **Flemyng E, Noel-Storr A, Macura B, et al.** *Position Statement on Artificial Intelligence (AI) Use in Evidence Synthesis Across Cochrane, the Campbell Collaboration, JBI, and the Collaboration for Environmental Evidence 2025.* Campbell Syst Rev 2025;21(4):e70074. DOI: [10.1002/cl2.70074](https://doi.org/10.1002/cl2.70074). Texto completo: [PMC12603384](https://pmc.ncbi.nlm.nih.gov/articles/PMC12603384/).
- **Walters WH, Wilder EI.** *Fabrication and errors in the bibliographic citations generated by ChatGPT.* Sci Rep 2023;13:14045. DOI: [10.1038/s41598-023-41032-5](https://doi.org/10.1038/s41598-023-41032-5). Texto completo: [PMC10484980](https://pmc.ncbi.nlm.nih.gov/articles/PMC10484980/).
- **Lieberum JL, Toews M, Metzendorf MI, et al.** *Large language models for conducting systematic reviews: on the rise, but not yet ready for use — a scoping review.* J Clin Epidemiol 2025;181:111746. DOI: [10.1016/j.jclinepi.2025.111746](https://doi.org/10.1016/j.jclinepi.2025.111746). Resumo: [PubMed 40021099](https://pubmed.ncbi.nlm.nih.gov/40021099/).
- **Castellanos A, Jiang H, Gomes P, Vander Meer D, Castillo A.** *Large Language Models for Thematic Summarization in Qualitative Health Care Research: Comparative Analysis of Model and Human Performance.* JMIR AI 2025;4:e64447. DOI: [10.2196/64447](https://doi.org/10.2196/64447). Texto completo: [PMC12231516](https://pmc.ncbi.nlm.nih.gov/articles/PMC12231516/).
- **Pizard S, Moreira R, Galiano F, Sastre I, Etcheverry L.** *On the Use of Large Language Models for Qualitative Synthesis.* arXiv:2510.16502 [cs.SE], 2025. **Preprint, sem revisão por pares.** [arxiv.org/abs/2510.16502](https://arxiv.org/abs/2510.16502).
- **RAISE — Responsible use of AI in evidence Synthesis.** Thomas J, Flemyng E, Noel-Storr A, et al. DOI: [10.17605/OSF.IO/FWAUD](https://doi.org/10.17605/OSF.IO/FWAUD).

---

*Documento produzido para a Issue #3. Dados de exemplo, quando houver, são fictícios.*
