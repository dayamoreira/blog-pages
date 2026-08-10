# ESSAY_COMMAND_CENTER

Painel de controle vivo da sua candidatura. Atualizado automaticamente toda vez que um essay for adicionado, planejado ou modificado através da skill `college-essay`.

**Status atual: 34 universidades registradas na lista-alvo** (ver nota de divergência de contagem abaixo) **· 0 essays com prompt/word limit definidos ainda.** Este documento está pronto para receber o primeiro essay assim que você fornecer, para qualquer uma destas universidades, o prompt e o word limit específicos.

*Última atualização: 10/08/2026.*

---

## ⚠️ Nota de verificação sobre a lista recebida

Antes de qualquer coisa, dois pontos que preciso sinalizar em vez de ignorar:

1. **Contagem:** o arquivo que você mandou se chama "35 Universidades", mas o array de dados tem **34 entradas** (9 REACH + 13 TARGET + 12 SAFETY). O card de resumo do próprio HTML diz "SAFETY: 13", mas só 12 universidades estão listadas no bloco `// SAFETY` do código. Registrei as 34 que existem de fato — se falta uma universidade de SAFETY, me diga qual para eu adicionar.
2. **Fonte dos dados (accept rate, SAT mid-50%, deadline):** registrei exatamente os números que vieram no seu arquivo, sem verificar cada um individualmente contra fonte oficial (Common Data Set / site de admissions de cada escola) — isso ficaria mais preciso se, quando chegarmos na etapa RESEARCH de cada universidade específica (via skill `college-essay`), confirmarmos accept rate e deadline reais no site oficial antes de finalizar qualquer essay. Os deadlines também não têm ano explícito — assumindo que são para o ciclo de transferência que começa agora (aplicações em torno de fev/mar/abr de 2027), mas vale confirmar.

---

## Nota metodológica

Este documento não substitui os outros oito — ele é o painel de controle que os conecta na prática, aplicação por aplicação, essay por essay. Toda linha da tabela principal deveria ser rastreável: a história a um código do `STORY_BANK.md`, a estrutura a uma entrada de `ESSAY_STRUCTURES.md`, o core trait a um dos sete listados em `APPLICANT_NARRATIVE.md`. Nada aqui deveria ser preenchido sem vir de uma decisão real tomada no workflow da skill `college-essay` — nenhuma célula desta tabela é aspiracional ou "provável", é o que foi de fato decidido.

**Como este documento é atualizado:** sempre que um essay passar por qualquer etapa do workflow de 14 passos (mesmo antes de terminar — por exemplo, assim que uma história for selecionada na etapa 4, já dá para registrar a linha com Status = "Story selected"), eu atualizo a tabela principal e recalculo as seis seções de análise abaixo. Você não precisa pedir para eu atualizar — isso deveria acontecer como parte natural de terminar qualquer etapa do workflow.

---

## University Registry (34)

Sua lista-alvo completa, organizada por tier (classificação sua, registrada como você forneceu). Esta tabela é o "cadastro" — a Tabela Principal abaixo é onde cada *essay* de cada universidade é rastreado individualmente, assim que houver prompt.

### 🚀 REACH (9) — accept rate 3–10%

| Universidade | Accept % | SAT Mid-50% | Localização | CS | Deadline | Essay status |
|---|---|---|---|---|---|---|
| Stanford University | 3.9% | 1500–1580 | Stanford, CA | Muito Forte | Mar 15 | Prompts pendentes |
| MIT | 4.6% | 1530–1580 | Cambridge, MA | Muito Forte | Mar 1 | Prompts pendentes |
| Harvard University | 4.2% | 1500–1580 | Cambridge, MA | Muito Forte | Mar 1 | Prompts pendentes |
| Yale University | 4.6% | 1490–1560 | New Haven, CT | Forte | Mar 1 | Prompts pendentes |
| Columbia University | 4.3% | 1490–1560 | New York, NY | Forte | Mar 1 | Prompts pendentes |
| Duke University | 5% | 1500–1570 | Durham, NC | Forte | Mar 1 | Prompts pendentes |
| Rice University | 7% | 1460–1560 | Houston, TX | Muito Forte | Mar 1 | Prompts pendentes |
| Johns Hopkins University | 8% | 1500–1570 | Baltimore, MD | Muito Forte | Mar 1 | Prompts pendentes |
| Tufts University | 10% | 1430–1540 | Medford, MA | Forte | Mar 1 | Prompts pendentes |

### 🎯 TARGET (13) — accept rate 10–25%

| Universidade | Accept % | SAT Mid-50% | Localização | CS | Deadline | Essay status |
|---|---|---|---|---|---|---|
| Cornell University | 8% | 1460–1550 | Ithaca, NY | Muito Forte | Mar 15 | Prompts pendentes |
| Vanderbilt University | 6% | 1460–1550 | Nashville, TN | Forte | Mar 15 | Prompts pendentes |
| Tulane University | 10% | 1350–1480 | New Orleans, LA | Médio | Mar 15 | Prompts pendentes |
| Grinnell College | 16% | 1330–1500 | Grinnell, IA | Médio | Mar 1 | Prompts pendentes |
| Emory University | 15% | 1420–1530 | Atlanta, GA | Forte | Mar 15 | Prompts pendentes |
| Northeastern University | 20% | 1380–1510 | Boston, MA | Forte | Mar 1 (Rolling) | Prompts pendentes |
| University of Michigan – Ann Arbor | 20% | 1370–1540 | Ann Arbor, MI | Muito Forte | Apr 15 (Rolling) | Prompts pendentes |
| University of North Carolina at Chapel Hill | 18% | 1360–1520 | Chapel Hill, NC | Forte | Mar 1 | Prompts pendentes |
| University of Texas at Austin | 20% | 1270–1490 | Austin, TX | Muito Forte | Mar 15 | Prompts pendentes |
| University of Virginia | 20% | 1370–1540 | Charlottesville, VA | Forte | Mar 1 | Prompts pendentes |
| Washington University in St. Louis | 11% | 1470–1560 | St. Louis, MO | Forte | Mar 15 | Prompts pendentes |
| Wellesley College | 24% | 1380–1510 | Wellesley, MA | Médio | Mar 1 | Prompts pendentes |
| New York University | 25% | 1410–1530 | New York, NY | Forte | Apr 1 (Rolling) | Prompts pendentes |

### 🛡️ SAFETY (12 — ver nota de contagem acima) — accept rate 25%+

| Universidade | Accept % | SAT Mid-50% | Localização | CS | Deadline | Essay status |
|---|---|---|---|---|---|---|
| Case Western Reserve University | 42% | 1340–1510 | Cleveland, OH | Forte | Mar 15 | Prompts pendentes |
| Stevens Institute of Technology | 32% | 1300–1500 | Hoboken, NJ | Forte | Mar 15 | Prompts pendentes |
| Brandeis University | 34% | 1350–1520 | Waltham, MA | Médio | Mar 15 | Prompts pendentes |
| University of Rochester | 30% | 1350–1510 | Rochester, NY | Forte | Mar 15 | Prompts pendentes |
| Purdue University | 53% | 1260–1470 | West Lafayette, IN | Muito Forte | Mar 1 | Prompts pendentes |
| University of Illinois Urbana-Champaign | 60% | 1300–1520 | Urbana, IL | Muito Forte | Mar 1 | Prompts pendentes |
| University of Maryland | 45% | 1320–1500 | College Park, MD | Forte | Mar 1 | Prompts pendentes |
| University of Massachusetts Amherst | 60% | 1260–1440 | Amherst, MA | Forte | Mar 1 | Prompts pendentes |
| University of Pittsburgh | 50% | 1300–1480 | Pittsburgh, PA | Forte | Mar 1 | Prompts pendentes |
| Virginia Tech | 70% | 1200–1420 | Blacksburg, VA | Muito Forte | Mar 1 | Prompts pendentes |
| Rochester Institute of Technology | 60% | 1250–1480 | Rochester, NY | Forte | Mar 15 | Prompts pendentes |
| Worcester Polytechnic Institute | 50% | 1310–1520 | Worcester, MA | Muito Forte | Mar 1 | Prompts pendentes |

### 💡 Observação fora da tabela: a coluna "Cheerleading" do seu arquivo original

Seu HTML tinha uma coluna inteira comparando força/inclusividade de cheerleading por escola — isso não é um dado neutro de admissions, é um sinal real de prioridade pessoal sua que ainda não está documentado em nenhum lugar do sistema. Isso conecta diretamente a algo que já está em `STORY_BANK.md` (S27): você mencionou querer participar de "experiências universitárias... de esportes a atividades estudantis" mas sentir "minha idade e meu corpo antes de qualquer outra característica minha". Vale uma pergunta direta: **cheerleading é algo que você já fez, quer tentar, ou é só um critério de ambiente de campus ao escolher escola?** Se houver uma história real aí, é um candidato forte para preencher a lacuna de "comunidade fora de contextos institucionais" já registrada em APPLICATION GAPS.

---

## Tabela Principal (por essay)

| University | Essay | Prompt | Word Limit | Category | Story | Structure | Core Trait | Status |
|---|---|---|---|---|---|---|---|---|
| *(aguardando o primeiro prompt — 34 universidades já cadastradas acima, nenhuma com essay iniciado)* | | | | | | | | |

---

## STORY USAGE MATRIX

Mostra em quais universidades/essays cada história do Story Bank já foi usada — o objetivo é enxergar rápido quais histórias estão sendo "gastas" e quais ainda estão disponíveis.

| Código | Nome curto | Força potencial | Usada em |
|---|---|---|---|
| S01 | As bonecas de pedra | 8 | — |
| S02 | Desmontar tudo | 7 | — |
| S03 | A porta de vidro | 9 | — |
| S04 | Os livros que minha mãe lia escondida | 7 | — |
| S05 | Minha mãe alfabetizando adultos na igreja | 6 | — |
| S06 | "Tira essas pretinhas daqui" | 9 | — |
| S07 | O avô que nunca conheci | 6 | — |
| S08 | Eu e Daniele contra o mundo | 5 | — |
| S09 | A luta pelo Curso Normal | 9 | — |
| S10 | A mudança para Maricá | 5 | — |
| S11 | Manhã, tarde e noite (2016) | 6 | — |
| S12 | O aluno que me ensinou a perguntar "por quê" | 9 | — |
| S13 | Consertando o Sims | 7 | — |
| S14 | O preço de vir para os EUA | 7 | — |
| S15 | A falta que sentia de pensar | 7 | — |
| S16 | A mesma frustração, país diferente | 8 | — |
| S17 | Fracassar era divertido | 9 | — |
| S18 | Danielle e a porta para o PhD | 8 | — |
| S19 | O primeiro F | 10 | — |
| S20 | O verão do GPA 4.0 | 6 | — |
| S21 | Refazer e vencer | 7 | — |
| S22 | Eu queria ter algo meu para apresentar | 6 | — |
| S23 | De perdida a presidente | 8 | — |
| S24 | Traduzir para 1.000 pessoas | 6 | — |
| S25 | Avaliar 200 ideias | 6 | — |
| S26 | Construir um sistema que decide quem é atendido primeiro | 5* | — |
| S27 | A vida que carrego junto com os estudos | 8 | — |
| S28 | O fio que conecta tudo (síntese, não história isolada) | N/A | — |

*S26: força 5 até a motivação pessoal ser esclarecida (ver Story Bank, pergunta pendente); potencial 9–10 depois.*

**Alerta automático:** se qualquer história aparecer em mais de uma linha da coluna "Usada em" **dentro da mesma universidade**, isso deveria disparar uma nota na seção REDUNDANCY ALERT abaixo. Entre universidades diferentes, reuso é normal (ver `COLLEGE_ESSAY_BLUEPRINT.md`, Regra Global 5).

---

## TRAIT COVERAGE MATRIX

Mostra quais dos 7 Core Traits (`APPLICANT_NARRATIVE.md`) já apareceram em algum essay, por universidade — para garantir que a candidatura como um todo mostre um retrato completo, não sempre os mesmos dois ou três traços.

| Core Trait | Evidência-base (Story Bank) | Aparece em |
|---|---|---|
| 1. Pensamento empírico aplicado à própria vida | S16, S19, S28 | — |
| 2. Insistência sem mapa pronto | S09, S23 | — |
| 3. Curiosidade sobre mecanismo, não resultado | S02, S12, S13, S17 | — |
| 4. Transformar falta pessoal em infraestrutura para outros | S05→S23, S12→S26, S24 | — |
| 5. Honestidade emocional sem dramatização | S27, S13 (autocorreção técnica) | — |
| 6. Reavaliação generosa do próprio passado | S01, S10, S16 | — |
| 7. Ambição que convive com medo | S22, S27, S28 | — |

**Alerta automático:** se, depois de várias universidades cadastradas, um trait nunca aparecer em "Aparece em", isso é um sinal de retrato incompleto — mais importante ainda se for o Trait 5 (honestidade emocional), que já é o menos explorado no banco atual segundo `APPLICANT_NARRATIVE.md`.

---

## STRUCTURE USAGE

Mostra quantas vezes cada arquitetura de `ESSAY_STRUCTURES.md` já foi escolhida — para evitar repetição mecânica da mesma estrutura em essays consecutivos, mesmo quando as histórias são diferentes.

| Estrutura | Vezes usada | Universidades |
|---|---|---|
| Narrative Arc | 0 | — |
| Montage / Portfólio | 0 | — |
| Circular Structure | 0 | — |
| Before / After | 0 | — |
| Problem → Exploration → Insight | 0 | — |
| Intellectual Journey | 0 | — |
| Thematic Structure | 0 | — |
| Reclamation / Redefinition | 0 | — |
| Manifesto + Prova Escalonada | 0 | — |
| Convergence Structure | 0 | — |
| Object-as-Lens | 0 | — |
| Escalation / Ceiling Structure | 0 | — |

**Alerta automático:** se uma mesma estrutura for escolhida 3+ vezes seguidas entre universidades diferentes, vale reconsiderar mesmo que cada história individualmente justifique aquela escolha — variedade estrutural entre essays ajuda o conjunto da candidatura a não parecer formulaico, mesmo que cada peça isoladamente esteja correta.

---

## REDUNDANCY ALERT

*Nenhum essay foi escrito ainda — nada a reportar.*

Quando houver essays cadastrados, esta seção lista automaticamente:
- Qualquer história usada em mais de um essay da mesma universidade.
- Qualquer core trait nomeado explicitamente (não só demonstrado) como tese central em mais de um essay da mesma universidade.
- Qualquer par de essays da mesma universidade que, mesmo com histórias diferentes, cheguem essencialmente à mesma reflexão final (ex.: dois essays diferentes ambos terminando em "decido com base em evidência, não em medo").

---

## APPLICATION GAPS

Características e dimensões importantes da Dayane que **ainda não aparecem em nenhum essay** — puxado diretamente das Missing Dimensions já documentadas em `APPLICANT_NARRATIVE.md` e do mapa de cobertura do `STORY_BANK.md`, ainda válidas porque nenhum essay foi escrito ainda:

1. **Humor leve, sem peso emocional por trás** — o banco tem humor (S03, S13), mas sempre junto de algo mais sério.
2. **A contradição "extrovertida mas antissocial"** — mencionada, nunca desenvolvida em cena.
3. **Comunidade fora de contextos institucionais** (bairro, comunidade brasileira em Boston, vida cotidiana) — tudo hoje é institucional (BHCC, PTK, Brazil Conference).
4. **A tutoria de CS no BHCC** (fato objetivo real, sem cena ainda) — provavelmente a lacuna mais fácil de preencher e mais valiosa para Leadership/Contribution.
5. **Uma decisão difícil recente/atual** — as documentadas (S09, S14) são todas de anos atrás.
6. **Interesse por arte** (Watercolor I, Digital Imaging for Artist, ambas A) — nunca mencionado na narrativa, pode não ser nada ou pode ser uma dimensão inteira ausente.
7. **Cheerleading** — descoberto agora, indiretamente, pela presença dessa coluna na sua planilha de universidades-alvo (ver nota na seção University Registry). Ainda não sei se é história, interesse atual, ou só critério de campus. Conecta com S27 (medo relacionado a idade/corpo em atividades estudantis).

Esta seção deveria encolher conforme universidades forem cadastradas e esses gaps forem preenchidos com histórias novas.

---

## RESEARCH GAPS

Essays Why Us / Why Major que ainda precisam de pesquisa institucional específica (ver `COLLEGE_ESSAY_BLUEPRINT.md`, Regra Global 6 — este Blueprint não pode fazer essa pesquisa sem uma universidade nomeada).

**34 universidades cadastradas, 0 com pesquisa institucional feita ainda.** Assim que um prompt de Why Us ou Why Major for fornecido para qualquer uma delas, essa universidade entra automaticamente na fila da etapa 1 (RESEARCH) do workflow da skill `college-essay`, seguindo o mesmo padrão de `ADMISSIONS_PRINCIPLES.md` (fontes oficiais, 🎓 vs. 🔍 separados). Como são 34 escolas, recomendo priorizar a pesquisa pela ordem em que os prompts forem chegando, não tentar pesquisar todas de uma vez.

**Lembrete permanente também registrado aqui:** a Bachelor's em Computer Science pela Descomplica (mai/2022–mai/2026, ver `STORY_BANK.md` linha do tempo e Pergunta 1) segue sem esclarecimento. Isso não é uma lacuna de pesquisa institucional, mas afeta diretamente qualquer essay de Transfer ou qualquer Why Major que narre a trajetória acadêmica completa — mantenho o lembrete aqui até ser resolvido.

---

## Legenda de ESSAY STATUS

| Status | Significa |
|---|---|
| **Not started** | Universidade/prompt registrado, nenhuma etapa do workflow iniciada. |
| **Research** | Etapa 1 (RESEARCH) em andamento ou concluída. |
| **Story selected** | Etapas 2–5 concluídas (Decode, Application Audit, Story Matching, Ranking) — história vencedora escolhida. |
| **Structure selected** | Etapa 6 (Structure Matching) concluída. |
| **Outline** | Etapas 7–8 concluídas (Angles, Outline) — esqueleto pronto, ainda sem prosa. |
| **Draft 1** | Etapa 9 (Draft) concluída — primeira versão escrita existe. |
| **Revision** | Em algum ponto das etapas 10–13 (Voice/Admissions/Redundancy/Cliché Check). |
| **Final** | Etapa 14 (Final Edit) concluída — pronto para submissão, ainda não enviado. |
| **Submitted** | Enviado à universidade. |

---

## Próximos passos

34 universidades já cadastradas no University Registry. O que falta para a Tabela Principal (por essay) começar a se preencher é você me passar, para qualquer uma delas, o **prompt específico + word limit** de um essay (personal statement via Common App, ou um supplement). Assim que isso chegar, eu aciono a skill `college-essay`, executo o workflow de 14 etapas, e a linha correspondente — mais as seis seções de análise — deixa de estar vazia. Dado o volume (34 escolas), pode fazer sentido priorizar o Personal Statement do Common App primeiro, já que ele provavelmente vale para a maioria destas universidades ao mesmo tempo.
