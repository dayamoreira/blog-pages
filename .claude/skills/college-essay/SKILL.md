---
name: college-essay
description: Workflow obrigatório de 14 etapas para planejar, estruturar e revisar college application essays da Dayane, usando como fontes de verdade os 9 documentos do sistema (ADMISSIONS_PRINCIPLES, ESSAY_ANALYSIS_DATABASE, ESSAY_STRUCTURES, WRITING_TECHNIQUES, STORY_BANK, APPLICANT_NARRATIVE, COLLEGE_ESSAY_BLUEPRINT, VOICE_PROFILE, ESSAY_COMMAND_CENTER). Use sempre que ela fornecer universidade + prompt + word limit e pedir para trabalhar em um essay de admissão — planejar, gerar ângulos, montar outline, escrever rascunho, ou revisar algo já escrito. Também use se ela mencionar "essay", "supplement", "personal statement", "why us", "why major" no contexto de aplicação para faculdade. Não use para cover letters de emprego (existe uma skill separada para isso) nem para nenhum outro tipo de texto.
---

# College Essay Workshop

Skill que transforma o sistema de 9 documentos construído nesta conta (pesquisa oficial de admissions + banco de essays reais analisados + taxonomia de estrutura + biblioteca de técnicas + banco de histórias pessoais da Dayane + síntese narrativa + blueprint estratégico + perfil de voz + command center com as 34 universidades-alvo) em um workflow executável, obrigatório e sempre na mesma ordem, toda vez que ela pedir ajuda com um essay de admissão específico.

## Quando usar esta skill

Invoque sempre que a Dayane fornecer **universidade + prompt + word limit** e pedir para:
- Planejar ou começar um essay novo.
- Escolher qual história usar para um prompt específico.
- Escrever um rascunho.
- Revisar um rascunho já existente (dela, não gerado por esta skill).

Se faltar universidade, prompt ou word limit, **pare e pergunte** antes de iniciar o workflow — essas três informações são obrigatórias para as etapas 1 (RESEARCH), 2 (DECODE) e 6 (STRUCTURE MATCHING). Não presuma nenhuma delas.

## Arquivos de referência (fontes de verdade)

Leia os arquivos relevantes de cada etapa antes de executá-la — não trabalhe de memória se o arquivo estiver desatualizado ou se a conversa for longa. Todos ficam na raiz do repositório:

| Arquivo | Papel no workflow |
|---|---|
| `ADMISSIONS_PRINCIPLES.md` | O que universidades dizem oficialmente que procuram — usado em RESEARCH, DECODE, ADMISSIONS CHECK. |
| `ESSAY_ANALYSIS_DATABASE.md` | Engenharia reversa de 15 essays reais admitidos — usado como referência de calibração em STORY MATCHING, RANKING e CLICHÉ CHECK. |
| `ESSAY_STRUCTURES.md` | Taxonomia de 12 arquiteturas narrativas/argumentativas — usado em STRUCTURE MATCHING. |
| `WRITING_TECHNIQUES.md` | Biblioteca de hooks, técnicas de corpo e endings, mais a seção de adaptação por word limit — usado em ANGLES, OUTLINE, DRAFT, FINAL EDIT. |
| `STORY_BANK.md` | As histórias reais da Dayane, cada uma com força potencial e riscos já avaliados — usado em STORY MATCHING e RANKING. |
| `APPLICANT_NARRATIVE.md` | Core traits, threads (intelectual/pessoal/contribuição), Redundancy Map, tensões preservadas — usado em RANKING, REDUNDANCY CHECK e ADMISSIONS CHECK. |
| `COLLEGE_ESSAY_BLUEPRINT.md` | Estratégia por categoria de essay (objetivo real, riscos, clichês comuns, o que evitar repetir) — usado em quase todas as etapas como referência central. |
| `VOICE_PROFILE.md` | Padrões reais da voz escrita/falada da Dayane — usado em VOICE CHECK. Ainda é uma primeira versão (duas amostras); atualize se surgir nova amostra de escrita dela. |
| `ESSAY_COMMAND_CENTER.md` | Painel vivo com as 34 universidades-alvo (tier, deadline, accept rate) e a tabela de todo essay em andamento — consultado no início de toda etapa (para saber o que já existe) e **atualizado automaticamente ao final de cada etapa** (ver seção própria abaixo). |

Se algum desses arquivos não existir ou estiver claramente desatualizado em relação à conversa atual, avise antes de continuar — não prossiga como se o arquivo dissesse algo que ele não diz.

---

## Workflow obrigatório (14 etapas, sempre nesta ordem)

Não pule etapas, não reordene, e não avance para DRAFT (etapa 9) sem ter completado 1–8 primeiro. Cada etapa produz um output visível antes de passar para a próxima — não silencie o processo, mostre o raciocínio de cada etapa como uma seção própria da resposta.

### 1. RESEARCH
Pesquise a universidade específica usando prioritariamente fontes oficiais (domínios `.edu` de admissions, páginas de "what we look for", páginas do departamento/major relevante) — seguindo o mesmo padrão de rigor de `ADMISSIONS_PRINCIPLES.md`: sempre separar **🎓 fonte oficial** de **🔍 análise própria**, sempre com link. Se o ambiente bloquear fetch direto de `.edu` (como aconteceu na construção deste sistema), use busca web e avise explicitamente essa limitação, como já documentado na nota metodológica de `ADMISSIONS_PRINCIPLES.md`.

### 2. DECODE
Explique o que o prompt está **realmente** tentando descobrir — não a leitura superficial da pergunta, a função admissions por trás dela. Cruze com `ADMISSIONS_PRINCIPLES.md` (qual categoria oficial esse prompt corresponde — Why Us, Why Major, Community, etc.) e com `COLLEGE_ESSAY_BLUEPRINT.md` (o que essa categoria já diz sobre "o que a universidade provavelmente tenta descobrir").

### 3. APPLICATION AUDIT
Pergunte à Dayane (ou revise o que já foi discutido na conversa) o que **já foi mostrado** em outras partes desta candidatura específica — outros essays já escritos para a mesma escola, atividades já listadas no resume/activities list, coisas já cobertas no transcript. O objetivo é identificar o que este essay específico **não pode** repetir. Se essa informação não estiver disponível, pergunte antes de seguir — não presuma que é a primeira peça da aplicação.

### 4. STORY MATCHING
Selecione de 3 a 5 histórias candidatas do `STORY_BANK.md` que respondem ao prompt decodificado na etapa 2. Cite o código de cada uma (`S0X`) e uma frase de por que ela é candidata.

### 5. RANKING
Dê nota a cada história candidata (pode ser 1–10 ou comparativa) considerando, explicitamente, estes seis critérios:
- **Fit com o prompt** (responde literalmente ao que foi perguntado)
- **Informação nova** (não repete o que a APPLICATION AUDIT da etapa 3 já revelou estar em outro lugar da aplicação)
- **Especificidade** (usa a força potencial e os detalhes memoráveis já registrados no Story Bank)
- **Potencial de reflexão** (a história permite chegar a um insight de segunda ordem, não só a uma "lição")
- **Autenticidade** (soa como a voz documentada em `VOICE_PROFILE.md`, não como uma versão performada da Dayane)
- **Memorabilidade** (o quanto fica na cabeça do leitor depois — geralmente correlacionado com especificidade, mas não sempre)

Mostre a comparação lado a lado, não só o resultado final.

### 6. STRUCTURE MATCHING
Consulte `ESSAY_STRUCTURES.md` e escolha 1–2 estruturas compatíveis com a história vencedora, o prompt e o word limit fornecido — usando explicitamente a seção "Como adaptar para diferentes word limits" desse arquivo. Nunca escolha uma estrutura só porque apareceu com frequência nos exemplos — justifique a escolha para esta história e este espaço específicos.

### 7. ANGLES
Antes de escrever qualquer coisa, gere 2–3 abordagens (ângulos) diferentes para a mesma história/estrutura — variando o que entra em foco (ex.: focar na cena vs. focar na reflexão; abrir pela ação vs. abrir por um objeto). Apresente as opções com um trade-off claro de cada uma. Não escolha por ela — pergunte qual ângulo ressoa antes de seguir para o outline, a menos que ela já tenha pedido explicitamente para você decidir.

### 8. OUTLINE
Só depois do ângulo escolhido: monte a estrutura detalhada do essay — parágrafo por parágrafo ou seção por seção, com a função de cada parte (hook, desenvolvimento, transição, reflexão, ending), consultando os campos "Sequência estrutural" e "Função de cada parte" da estrutura escolhida em `ESSAY_STRUCTURES.md`. Ainda sem prosa final — isto é esqueleto, não rascunho.

### 9. DRAFT
**Só escreva depois que outline e direção estiverem definidos e aprovados.** O rascunho deve:
- Usar exclusivamente fatos, detalhes e falas já registrados no `STORY_BANK.md` — nada novo pode aparecer aqui que não estivesse lá ou que ela não tenha acabado de fornecer.
- Seguir a estrutura do outline da etapa 8.
- Aplicar as técnicas de hook/corpo/ending escolhidas, consultando `WRITING_TECHNIQUES.md`.
- Respeitar o word limit fornecido.

### 10. VOICE CHECK
Compare o rascunho com `VOICE_PROFILE.md`, item por item (ver a seção "Como usar no VOICE CHECK" desse arquivo): frases longas demais, metáfora sustentada aparecendo sem necessidade, reflexão introduzida por frases-clichê de transição, linguagem elevada em momentos que pediriam honestidade seca. Marque trechos específicos, não uma avaliação genérica.

### 11. ADMISSIONS CHECK
Releia o rascunho e responda explicitamente: **o que um leitor aprende sobre a Dayane ao final deste texto?** Compare essa resposta com o campo "O que um leitor deveria aprender ao final" da categoria correspondente em `COLLEGE_ESSAY_BLUEPRINT.md`. Se não bater, isso é um problema a resolver antes do Final Edit, não depois.

### 12. REDUNDANCY CHECK
Compare com os outros essays já escritos **para a mesma aplicação** (ver Regra Global 5 de `COLLEGE_ESSAY_BLUEPRINT.md` e o Redundancy Map de `APPLICANT_NARRATIVE.md`). Sinalize qualquer história, frase-tese ("insisti sem mapa", "sou curiosa") ou trait nomeado que já apareceu em outro essay desta mesma escola.

### 13. CLICHÉ CHECK
Releia especificamente atrás de frases ou ideias genéricas — cruzando com os clichês documentados por categoria em `COLLEGE_ESSAY_BLUEPRINT.md` e com os "erros comuns" oficiais de `ADMISSIONS_PRINCIPLES.md` (seção 12). Marque cada ocorrência encontrada.

### 14. FINAL EDIT
Melhore clareza, ritmo, estrutura e concisão — **sem artificializar a voz**. Qualquer mudança de frase precisa passar pelo mesmo teste do VOICE CHECK (etapa 10). Entregue a versão final junto com um resumo curto do que mudou entre o rascunho (etapa 9) e esta versão, e por quê.

---

## Atualização automática do ESSAY_COMMAND_CENTER.md

O Command Center não se atualiza sozinho — é uma responsabilidade desta skill, não um pedido separado que a Dayane precisa fazer toda vez. Sempre que qualquer etapa do workflow acima for concluída para um essay (mesmo que o essay inteiro ainda não esteja pronto), atualize no mesmo turno:

- **Tabela Principal:** crie ou atualize a linha (University, Essay, Prompt, Word Limit, Category, Story, Structure, Core Trait, Status) assim que cada uma dessas informações for decidida — não espere o essay terminar para registrar. O `Status` segue a legenda do próprio Command Center (Not started → Research → Story selected → Structure selected → Outline → Draft 1 → Revision → Final → Submitted).
- **Story Usage Matrix:** adicione a universidade/essay na coluna "Usada em" da história escolhida assim que a etapa 5 (RANKING) definir a vencedora.
- **Trait Coverage Matrix:** marque o core trait correspondente assim que ele for identificado (geralmente junto com a etapa 11, ADMISSIONS CHECK).
- **Structure Usage:** incremente o contador da estrutura escolhida na etapa 6.
- **Redundancy Alert:** preencha ou atualize se a etapa 12 (REDUNDANCY CHECK) encontrar alguma colisão dentro da mesma universidade.
- **Application Gaps / Research Gaps:** remova um item quando ele deixar de ser lacuna (ex.: uma história nova preenche um gap; uma universidade tem sua etapa RESEARCH concluída).

Mostre essa atualização como parte visível da resposta (não é um passo silencioso) — mas não é preciso repetir o Command Center inteiro a cada vez, só a mudança feita.

---

## Regras absolutas (nunca violar, em nenhuma etapa)

1. **Nunca inventar fatos, sentimentos ou diálogos.** Se um detalhe necessário não existir no `STORY_BANK.md`, pare e pergunte — não preencha a lacuna.
2. **Nunca aumentar dramaticamente uma história.** A força de uma história vem da especificidade real, não da intensidade artificial.
3. **Nunca copiar essays existentes.** `ESSAY_ANALYSIS_DATABASE.md` e `ESSAY_STRUCTURES.md` existem para ensinar técnica e arquitetura reutilizáveis — não frases, metáforas ou estruturas de frase específicas de outro autor.
4. **Nunca escrever algo apenas porque soa impressionante.** Toda escolha de conteúdo ou frase precisa servir ao prompt e à voz da Dayane, não a uma impressão de sofisticação.
5. **Preservar a maneira natural dela de pensar e se expressar** — ver `VOICE_PROFILE.md` a cada etapa relevante, não só no VOICE CHECK.
6. **Mostrar características através de ações sempre que possível** — usar a técnica Showing vs. Telling (`WRITING_TECHNIQUES.md`) em vez de declarar traços.
7. **Priorizar detalhes específicos** — usar o campo "Detalhes memoráveis" de cada história do Story Bank como material preferencial sobre generalização.
8. **Não transformar todo essay em trauma ou superação.** O Story Bank tem histórias leves, curiosas, técnicas e cômicas — usar a variedade real, não sempre a mais "dramática" disponível.
9. **Não repetir a mesma história sem necessidade** — aplicar a Regra Global 5 de `COLLEGE_ESSAY_BLUEPRINT.md` em toda etapa de RANKING e REDUNDANCY CHECK.
10. **Estrutura é ferramenta, não fórmula.** Nunca force uma história dentro de uma arquitetura de `ESSAY_STRUCTURES.md` só porque ela é comum ou porque apareceu em outro essay — se nenhuma estrutura catalogada servir bem, isso deveria ser dito explicitamente, não escondido.

## O que fazer quando uma etapa expõe uma lacuna

Se, em qualquer etapa (mais provável em STORY MATCHING ou DRAFT), ficar claro que falta um detalhe que o `STORY_BANK.md` não tem — pare a etapa, formule a pergunta de follow-up específica (no mesmo formato já usado nesse arquivo: "O que aconteceu exatamente? Onde você estava? Quem estava lá?..."), e só retome o workflow depois da resposta. Isso vale mesmo que atrase a entrega do essay — é preferível a inventar.
