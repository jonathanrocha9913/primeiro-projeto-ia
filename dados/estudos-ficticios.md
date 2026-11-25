# Conjunto fictício de estudos (Issue #5)

Planilha de teste do app de síntese: **10 estudos inventados**, uma linha por estudo, no formato
de extração de dados de uma revisão sistemática. Serve para alimentar o protótipo e os testes
automatizados do MVP.

> **Aviso.** Todos os estudos, autores, revistas, números e trechos deste arquivo são
> **fictícios**, criados para teste. Não correspondem a pessoas, pacientes, estudantes ou
> pesquisas reais. Os sobrenomes (Quimera, Zabelê, Orvalho, Ventania, Miragem, Siriguela,
> Borduna, Taperoá, Candeia, Cajuína) foram escolhidos justamente para não serem confundidos
> com autores reais — qualquer semelhança é coincidência.

- **Arquivo de dados:** `dados/estudos-ficticios.csv`
- **Formato:** CSV, codificação **UTF-8 sem BOM**, separador **ponto e vírgula** (`;`).
  No Excel em português o arquivo abre direto; no Google Sheets ou no Numbers, escolha a
  importação com separador `;`.
- **Tamanho:** 10 linhas de dados + 1 linha de cabeçalho, 18 colunas.

## Tema da revisão fictícia

A pergunta simulada é: *intervenções digitais de apoio ao autocuidado (mensagens, ligações,
aplicativos, telemonitoramento) melhoram desfechos de adultos com hipertensão na atenção
primária?* Todos os estudos giram em torno dela, mas medem desfechos diferentes — o que é
comum em uma extração real.

## Colunas

| Coluna | O que guarda | Exemplo |
|---|---|---|
| `id_estudo` | Identificador curto do estudo | `FIC-01` |
| `autor_ano` | Autoria e ano (fictícios) | `Quimera & Borduna (2018)` |
| `pais` | País do estudo | `Brasil` |
| `desenho` | Tipo de estudo | `Ensaio clínico randomizado` |
| `populacao` | Quem foi estudado | `Adultos com hipertensão arterial na atenção primária` |
| `amostra` | Número de participantes | `240` |
| `intervencao` | O que foi testado | `Lembrete por SMS duas vezes por semana` |
| `comparador` | Com o que foi comparado | `Cuidado usual` |
| `desfecho` | O que foi medido | `Pressão arterial sistólica (mmHg) após 6 meses` |
| `tema` | Tema sugerido na planilha (pode ficar vazio) | `Controle pressórico` |
| `direcao` | Sentido do resultado: `a favor`, `contra`, `neutro` ou `não se aplica` | `a favor` |
| `resultado` | O resultado em uma frase | `Queda de 6,4 mmHg...` |
| `medida_efeito` | Número principal | `Diferença de médias: -4,5 mmHg` |
| `ic95` | Intervalo de confiança de 95% | `-7,1 a -1,9` |
| `valor_p` | Valor de p | `0,001` |
| `trecho_fonte` | Trecho do artigo que sustenta o achado | `a pressão arterial sistólica caiu...` |
| `localizacao_fonte` | Onde o trecho está no artigo | `p. 6, Resultados, 2º parágrafo` |
| `observacoes` | Notas do revisor | `Estudo fictício...` |

## O que cada linha testa

| ID | Estudo | Desfecho | O que a linha testa |
|---|---|---|---|
| FIC-01 | Quimera & Borduna (2018) | Pressão sistólica | Base do **par repetido 1** (mesmo achado de FIC-05). |
| FIC-02 | Zabelê, Orvalho & Candeia (2020) | Adesão por registro de dispensação (MPR) | Base do **par repetido 2** (mesmo achado de FIC-07). |
| FIC-03 | Orvalho & Taperoá (2019) | Faltas em consultas | Metade do **par conflitante**: aqui o lembrete reduz as faltas. |
| FIC-04 | Ventania, Siriguela & Miragem (2021) | Conhecimento sobre a doença | Achado isolado, com medida de efeito e IC; nenhum par. |
| FIC-05 | Borduna & Cajuína (2022) | Pressão sistólica | **Par repetido 1**: mesma conclusão de FIC-01, com outras palavras e outra forma de apresentar o número. |
| FIC-06 | Zabelê & Ventania (2017) | Qualidade de vida (SF-12) | **Resultado nulo** relatado como nulo: o app não deve transformar "sem diferença" em efeito. |
| FIC-07 | Miragem, Quimera & Zabelê (2023) | Adesão autorreferida | **Par repetido 2**: mesma conclusão de FIC-02, com métrica e redação diferentes. |
| FIC-08 | Siriguela, Candeia & Taperoá (2020) | Faltas em consultas | **Par conflitante** com FIC-03: mesmo desfecho, conclusão oposta. |
| FIC-09 | Cajuína & Miragem (2024) | Aceitação e engajamento | **Achado ambíguo**: a planilha não tem trecho literal, só um resumo do revisor, e não há número. |
| FIC-10 | Taperoá, Siriguela & Orvalho (2019) | Frequência de medida em casa | **Tema em branco**: precisa cair no grupo "sem tema" sem perder a linha. |

## Gabarito dos testes plantados

- **Par repetido 1 — FIC-01 e FIC-05.** Os dois mostram queda da pressão sistólica com apoio
  digital (cerca de 6 a 7 mmHg a mais que o comparador). FIC-01 fala em "diferença de -4,5 mmHg
  entre grupos"; FIC-05 fala em "queda de 7,3 mmHg contra 0,8 mmHg". Mesma conclusão, redação e
  números diferentes. É o caso que o app precisa aproximar por **tema + sentido do resultado**,
  não por igualdade de texto.
- **Par repetido 2 — FIC-02 e FIC-07.** Os dois mostram adesão maior com mensagens de texto.
  FIC-02 mede doses dispensadas (MPR 0,86 contra 0,71); FIC-07 mede autorrelato (78% contra 63%).
  Mesma conclusão, métricas diferentes — o app deve sinalizar a repetição **e** deixar visível
  que a forma de medir mudou (isso é material para a seção de limitações).
- **Conflito — FIC-03 e FIC-08.** Mesmo desfecho (faltas em consultas) e sentidos opostos:
  FIC-03 reduz de 40% para 22% (RR 0,55); FIC-08 fica em 31% contra 29% (RR 1,07, sem
  significância). Não é repetição de achado: é contradição, e o prompt de verificação precisa
  apontar os dois estudos.
- **Ambíguo — FIC-09.** O campo `trecho_fonte` diz explicitamente que não há citação literal e
  que o conteúdo é um resumo do revisor. `medida_efeito`, `ic95` e `valor_p` estão vazios,
  `direcao` é `não se aplica`. O app não pode inventar trecho nem número: deve mostrar o achado
  como frágil e pedir conferência no artigo.
- **Sem tema — FIC-10.** `tema` vazio. O achado existe, tem número e trecho, e precisa aparecer
  no grupo "sem tema" (ou equivalente), não desaparecer.
- **Resultado nulo — FIC-06.** `direcao` é `neutro` e o IC cruza zero. O app não deve apresentar
  isso como benefício.
- **Linhas sem par — FIC-04, FIC-06, FIC-09 e FIC-10.** Não devem ser marcadas como repetição.
  Se o app marcar, é falso positivo — e o teste de sucesso do MVP (Issue #6) falha.

## Como conferir rapidamente

1. O arquivo tem 10 linhas de dados e nenhum `id_estudo` repetido.
2. Os IDs vão de `FIC-01` a `FIC-10`.
3. Existem exatamente **dois** pares de achados com a mesma conclusão: (FIC-01, FIC-05) e
   (FIC-02, FIC-07).
4. Existe **um** par com a mesma pergunta e conclusão oposta: (FIC-03, FIC-08).
5. Existe **um** achado sem trecho literal: FIC-09.
6. Existe **uma** linha sem tema: FIC-10.
7. Nenhum nome, número ou trecho corresponde a pessoa ou estudo real.

## Privacidade

Nenhum dado real de paciente, estudante ou participante foi usado. Se um dia este conjunto for
substituído por dados de pesquisa reais, isso exige avaliação de LGPD, segurança e, quando
cabível, comitê de ética antes de qualquer uso com modelos de IA ou publicação no GitHub.
