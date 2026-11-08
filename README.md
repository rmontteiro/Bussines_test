# bussines_test

[Português (Brasil)](#português-brasil) · [Español (Argentina)](#español-argentina) · [English (US)](#english-us)

<a id="português-brasil"></a>
## Português (Brasil)

### Sobre

**bussines_test** é uma skill de instruções reutilizáveis para avaliar ideias de negócio com análise estratégica, pesquisa de mercado e questionamento crítico. Seu objetivo é transformar uma ideia em uma decisão fundamentada e em um plano prático de validação.

Foi concebida para uso com **Cursor, Claude, Gemini, Qwen e ChatGPT**. A compatibilidade se dá pelo uso de instruções em texto; instalação nativa, acesso à internet e ferramentas disponíveis dependem do produto, da versão e do plano.

### Quando usar

- Avaliar um negócio, produto, serviço ou oportunidade.
- Identificar premissas frágeis, concorrentes e riscos.
- Examinar monetização, custos e viabilidade operacional.
- Definir um MVP e experimentos de baixo custo.
- Decidir entre avançar, testar, pivotar ou abandonar.

### As 13 áreas de análise

1. **Análise fundamental:** problema, solução, premissas e lacunas.
2. **Validação de mercado:** público, demanda, tamanho de mercado e tendências.
3. **Modelo de negócios:** receita, custos, economia unitária e lucratividade.
4. **Realidades operacionais:** equipe, recursos, tecnologia e regulação.
5. **Cenário competitivo:** concorrentes, substitutos e diferenciação.
6. **Análise de risco:** dez riscos prioritários, sinais de alerta e mitigação.
7. **Melhor cenário:** resultados possíveis em 1, 3 e 5 anos e suas condições.
8. **Pior cenário:** modos de fracasso, exposição e limites de perda.
9. **Roteiro de validação:** hipóteses, experimentos, métricas e critérios.
10. **Requisitos de execução:** MVP, responsáveis, cronograma e lançamento.
11. **Nomeação e posicionamento:** nomes, proposta de valor e comunicação.
12. **Recomendações de melhoria:** ajustes, parcerias e vantagens defensáveis.
13. **Decisão GO/NO-GO:** nota de viabilidade, confiança e próximos passos.

### Como usar

As instruções da skill estão disponíveis em [SKILL.md](SKILL.md). Este README documenta seu uso; sozinho, não instala nem ativa a skill.

| Ferramenta | Aplicação |
| --- | --- |
| Cursor | Adicione o arquivo ao projeto e peça ao agente para lê-lo. Para uso persistente, configure uma regra que faça referência ao arquivo. |
| Claude | Use o recurso de skills onde estiver disponível ou adicione o conteúdo às instruções do projeto. |
| Gemini | Cole o conteúdo nas instruções de um Gem ou forneça o arquivo na conversa. |
| Qwen | Use instruções personalizadas, contexto de arquivo ou uma mensagem de sistema na integração, conforme o produto. |
| ChatGPT | Use instruções de um GPT ou projeto, ou anexe o arquivo e peça sua aplicação. |

Não é necessário usar as cinco IAs ao mesmo tempo. A skill pode ser executada por um único assistente. Comparações entre modelos devem usar o mesmo contexto e preservar a origem de cada contribuição.

### Ativação pelo chat — copie e cole

Cole o bloco da ferramenta escolhida diretamente na janela de diálogo. Não é necessário abrir um terminal nem clonar o repositório. **Nome:** `bussines_test`. **Identificador técnico:** `bussines-test`.

O assistente precisa conseguir ler o link ou receber o arquivo. Em modos de agente com acesso a arquivos, o pedido também autoriza salvar a skill no projeto atual. Em chats comuns, o efeito se limita à conversa; persistência entre conversas depende das configurações de projeto, Gem, GPT ou skills disponíveis na interface.

#### Cursor — chat do Agent

```text
Configure a skill bussines_test neste projeto usando o identificador bussines-test.

Leia o conteúdo completo de:
https://raw.githubusercontent.com/rmontteiro/Bussines_test/main/SKILL.md

Salve uma cópia fiel em .cursor/skills/bussines-test/SKILL.md no projeto atual. Se já existir, compare os conteúdos e preserve alterações locais: mostre as diferenças e peça minha decisão antes de substituí-las. Verifique o frontmatter e o caminho. Use suas ferramentas para realizar a configuração, sem me pedir que execute comandos no terminal.

Aplique a skill nesta conversa e responda em português do Brasil. Informe o que foi salvo e se a descoberta nativa foi verificada ou ainda depende de uma nova sessão. Se não conseguir acessar o link ou gravar arquivos, explique a limitação e peça o SKILL.md anexado ou colado, sem afirmar que instalou. Aguarde minha ideia de negócio.
```

#### Claude — chat ou Claude Code

```text
Quero usar a skill bussines_test, identificador bussines-test.

Leia o conteúdo completo de:
https://raw.githubusercontent.com/rmontteiro/Bussines_test/main/SKILL.md

Se estiver no Claude Code com acesso ao projeto, salve uma cópia fiel em .claude/skills/bussines-test/SKILL.md e verifique o arquivo. Antes de substituir uma versão com alterações locais, mostre as diferenças e peça minha decisão. Faça a configuração com suas ferramentas, sem me pedir comandos de terminal.

Se estiver no chat web ou sem acesso ao projeto, aplique as instruções nesta conversa. Não afirme que houve instalação persistente. Se eu quiser reutilizar em outras conversas, explique como adicionar o arquivo e uma instrução para consultá-lo ao projeto ou ao recurso de skills disponível na interface.

Responda em português do Brasil. Se não conseguir ler o link, peça que eu anexe ou cole o SKILL.md. Confirme apenas o que realmente realizou e aguarde minha ideia de negócio.
```

#### Gemini — chat, Gem ou Gemini CLI

```text
Ative a skill bussines_test, identificador bussines-test, a partir do conteúdo completo deste arquivo:
https://raw.githubusercontent.com/rmontteiro/Bussines_test/main/SKILL.md

Se estiver no Gemini CLI com acesso ao projeto, salve uma cópia fiel em .gemini/skills/bussines-test/SKILL.md. Verifique o arquivo e, se houver recurso disponível, atualize a descoberta de skills. Antes de substituir alterações locais, mostre as diferenças e peça minha decisão. Execute a configuração com suas ferramentas, sem me pedir comandos de terminal.

Se estiver no Gemini web ou em um Gem sem acesso ao projeto, siga a skill nesta conversa. Para persistência, explique como incluir as instruções na configuração de um Gem; não declare que essa configuração foi feita sem realmente realizá-la.

Responda em português do Brasil. Se não puder ler o link, peça o SKILL.md anexado ou colado. Distinga arquivo salvo de skill descoberta e aguarde minha ideia de negócio.
```

#### Qwen — chat ou Qwen Code

```text
Configure e aplique a skill bussines_test, identificador bussines-test.

Leia o conteúdo completo de:
https://raw.githubusercontent.com/rmontteiro/Bussines_test/main/SKILL.md

Se estiver no Qwen Code com acesso ao projeto, salve uma cópia fiel em .qwen/skills/bussines-test/SKILL.md e verifique o arquivo. Preserve alterações locais: mostre diferenças e peça minha decisão antes de substituí-las. Faça a configuração com suas ferramentas, sem me pedir comandos de terminal.

Se estiver no Qwen Chat ou sem acesso a arquivos, aplique a skill apenas nesta conversa. Não afirme que criou uma instalação persistente. Para reutilização, indique as opções de personalização realmente disponíveis na interface.

Responda em português do Brasil. Se não conseguir abrir o link, peça que eu anexe ou cole o SKILL.md. Informe o resultado real da configuração e aguarde minha ideia de negócio.
```

#### ChatGPT — conversa, projeto ou GPT

```text
Quero aplicar a skill bussines_test nesta conversa.

Abra e leia o conteúdo completo de:
https://raw.githubusercontent.com/rmontteiro/Bussines_test/main/SKILL.md

Siga as instruções da skill para as próximas análises de negócio nesta conversa e responda em português do Brasil. Se não conseguir acessar o conteúdo completo, peça que eu anexe ou cole o SKILL.md antes de afirmar que a skill foi carregada.

Não afirme que instalou uma extensão, alterou minha memória ou configurou outros chats. Se eu quiser persistência, oriente-me a adicionar o SKILL.md aos arquivos de um projeto, ou ao conhecimento de um GPT quando disponível, e a incluir uma instrução explícita para consultá-lo.

Confirme a leitura somente se ela ocorreu e aguarde minha ideia de negócio.
```

#### Se o link não abrir

Abra [SKILL.md](SKILL.md) no GitHub e anexe o arquivo ou cole seu conteúdo completo na mesma conversa. Depois, repita o pedido de aplicação. O endereço do repositório, sozinho, não garante que a ferramenta tenha lido a skill.

#### Verificação e atualização pelo chat

Após a confirmação, envie o exemplo abaixo. Para atualizar, cole novamente o bloco da ferramenta e peça que releia a versão atual do link. Nos agentes com arquivos, confirme eventuais substituições após revisar as diferenças. Em projetos, Gems ou GPTs configurados manualmente, atualize também o arquivo ou as instruções pela interface.

Os textos acima são pedidos em linguagem natural, não comandos nativos de instalação. A configuração depende das ferramentas e permissões da sessão; não foi testada dentro dos cinco aplicativos.

### Exemplo de solicitação

```text
Leia e aplique a skill bussines_test em modo completo.
Responda em português do Brasil.

Ideia: assinatura de refeições prontas para profissionais em trabalho remoto.
Público e região: profissionais que moram sozinhos em São Paulo.
Estágio: ideia, sem vendas.
Orçamento e prazo: R$ 10.000 para um piloto de 60 dias.
Evidências existentes: cinco conversas exploratórias; nenhuma pré-venda.
Principal dúvida: como testar disposição de pagamento antes de montar a operação?

Faça as perguntas críticas necessárias. Avance com uma análise preliminar
quando possível, deixando claras as premissas e as limitações.
```

### Resultado esperado e princípios

A resposta deve trazer resumo executivo, análise das 13 áreas, riscos prioritários e experimentos com hipótese, público, prazo, custo, métrica e limiar de aprovação. Deve terminar com três ações prioritárias e uma recomendação: **GO**, **TESTAR**, **PIVOTAR** ou **NO-GO**.

Fatos, informações do usuário, hipóteses e estimativas devem ser diferenciados. Dados externos precisam de fontes verificáveis; projeções precisam de premissas e cálculos. Sem acesso a pesquisa, o assistente deve explicar a limitação e indicar como obter evidências.

A nota de viabilidade de 1 a 10 não é uma probabilidade de sucesso. Nomes sugeridos precisam de verificação de marca e domínio. Questões jurídicas e regulatórias dependem da jurisdição e de verificação apropriada.

---

<a id="español-argentina"></a>
## Español (Argentina)

### Acerca de la skill

**bussines_test** es una skill de instrucciones reutilizables para evaluar ideas de negocio mediante análisis estratégico, investigación de mercado y revisión crítica. Su objetivo es convertir una idea en una decisión fundamentada y un plan concreto de validación.

Está pensada para **Cursor, Claude, Gemini, Qwen y ChatGPT**. La compatibilidad se basa en instrucciones de texto; la instalación nativa, el acceso a internet y las herramientas disponibles dependen del producto, la versión y el plan.

### Cuándo usarla

- Evaluar un negocio, producto, servicio u oportunidad.
- Detectar supuestos débiles, competidores y riesgos.
- Revisar monetización, costos y viabilidad operativa.
- Definir un MVP y experimentos de bajo costo.
- Decidir si avanzar, validar, pivotear o abandonar.

### Las 13 áreas de análisis

1. **Análisis fundamental:** problema, solución, supuestos y brechas.
2. **Validación de mercado:** público, demanda, tamaño de mercado y tendencias.
3. **Modelo de negocio:** ingresos, costos, economía unitaria y rentabilidad.
4. **Realidad operativa:** equipo, recursos, tecnología y regulación.
5. **Panorama competitivo:** competidores, sustitutos y diferenciación.
6. **Análisis de riesgos:** diez riesgos prioritarios, alertas y mitigación.
7. **Mejor escenario:** resultados posibles a 1, 3 y 5 años y sus condiciones.
8. **Peor escenario:** formas de fracaso, exposición y límites de pérdida.
9. **Plan de validación:** hipótesis, experimentos, métricas y criterios.
10. **Requisitos de ejecución:** MVP, responsables, cronograma y lanzamiento.
11. **Nombre y posicionamiento:** nombres, propuesta de valor y comunicación.
12. **Recomendaciones de mejora:** ajustes, alianzas y ventajas defendibles.
13. **Decisión GO/NO-GO:** puntaje de viabilidad, confianza y próximos pasos.

### Cómo usarla

Las instrucciones de la skill están disponibles en [SKILL.md](SKILL.md). Este README explica su uso; por sí solo no instala ni activa la skill.

| Herramienta | Aplicación |
| --- | --- |
| Cursor | Agregá el archivo al proyecto y pedile al agente que lo lea. Para uso persistente, configurá una regla que haga referencia al archivo. |
| Claude | Usá la función de skills donde esté disponible o agregá el contenido a las instrucciones del proyecto. |
| Gemini | Pegá el contenido en las instrucciones de un Gem o adjuntá el archivo en la conversación. |
| Qwen | Usá instrucciones personalizadas, contexto de archivo o un mensaje de sistema en la integración, según el producto. |
| ChatGPT | Usá las instrucciones de un GPT o proyecto, o adjuntá el archivo y pedí que se aplique. |

No hace falta usar las cinco IAs al mismo tiempo. Un solo asistente puede ejecutar la skill. Para comparar modelos, usá el mismo contexto e identificá el origen de cada aporte.

### Activación por chat — copiá y pegá

Pegá el bloque de la herramienta elegida directamente en su ventana de diálogo. No hace falta abrir una terminal ni clonar el repositorio. **Nombre:** `bussines_test`. **Identificador técnico:** `bussines-test`.

El asistente necesita leer el enlace o recibir el archivo. En modo agente con acceso a archivos, el pedido también autoriza guardar la skill en el proyecto actual. En un chat común, el efecto se limita a la conversación; la persistencia depende de las opciones de proyecto, Gem, GPT o skills de la interfaz.

#### Cursor — chat de Agent

```text
Configurá la skill bussines_test en este proyecto con el identificador bussines-test.

Leé el contenido completo de:
https://raw.githubusercontent.com/rmontteiro/Bussines_test/main/SKILL.md

Guardá una copia fiel en .cursor/skills/bussines-test/SKILL.md dentro del proyecto actual. Si existe, compará los contenidos y preservá los cambios locales: mostrá las diferencias y pedime una decisión antes de reemplazarlos. Verificá el frontmatter y la ruta. Usá tus herramientas para configurarla, sin pedirme comandos de terminal.

Aplicá la skill en esta conversación y respondé en español de Argentina. Indicá qué guardaste y si verificaste el descubrimiento nativo o si requiere una sesión nueva. Si no podés leer el enlace o escribir archivos, explicá la limitación y pedime el SKILL.md adjunto o pegado. No afirmes que instalaste algo sin hacerlo. Esperá mi idea de negocio.
```

#### Claude — chat o Claude Code

```text
Quiero usar la skill bussines_test, identificador bussines-test.

Leé el contenido completo de:
https://raw.githubusercontent.com/rmontteiro/Bussines_test/main/SKILL.md

Si estás en Claude Code con acceso al proyecto, guardá una copia fiel en .claude/skills/bussines-test/SKILL.md y verificá el archivo. Antes de reemplazar una versión con cambios locales, mostrá las diferencias y pedime una decisión. Usá tus herramientas, sin pedirme comandos de terminal.

Si estás en el chat web o sin acceso al proyecto, aplicá las instrucciones en esta conversación. No afirmes que hay una instalación persistente. Para reutilizarla, explicá cómo agregar el archivo y una instrucción para consultarlo al proyecto o a la función de skills disponible.

Respondé en español de Argentina. Si no podés leer el enlace, pedime que adjunte o pegue el SKILL.md. Confirmá solo lo que hiciste y esperá mi idea de negocio.
```

#### Gemini — chat, Gem o Gemini CLI

```text
Activá la skill bussines_test, identificador bussines-test, usando el contenido completo de:
https://raw.githubusercontent.com/rmontteiro/Bussines_test/main/SKILL.md

Si estás en Gemini CLI con acceso al proyecto, guardá una copia fiel en .gemini/skills/bussines-test/SKILL.md. Verificá el archivo y actualizá el descubrimiento de skills si tenés esa función disponible. Antes de reemplazar cambios locales, mostrá las diferencias y pedime una decisión. Usá tus herramientas, sin pedirme comandos de terminal.

Si estás en Gemini web o en un Gem sin acceso al proyecto, seguí la skill en esta conversación. Para persistencia, explicá cómo incluir las instrucciones en la configuración de un Gem; no afirmes que lo configuraste sin hacerlo.

Respondé en español de Argentina. Si no podés leer el enlace, pedime el SKILL.md adjunto o pegado. Diferenciá archivo guardado de skill descubierta y esperá mi idea de negocio.
```

#### Qwen — chat o Qwen Code

```text
Configurá y aplicá la skill bussines_test, identificador bussines-test.

Leé el contenido completo de:
https://raw.githubusercontent.com/rmontteiro/Bussines_test/main/SKILL.md

Si estás en Qwen Code con acceso al proyecto, guardá una copia fiel en .qwen/skills/bussines-test/SKILL.md y verificá el archivo. Preservá cambios locales: mostrá diferencias y pedime una decisión antes de reemplazarlos. Usá tus herramientas, sin pedirme comandos de terminal.

Si estás en Qwen Chat o sin acceso a archivos, aplicá la skill solo en esta conversación. No afirmes que creaste una instalación persistente. Para reutilizarla, indicá las opciones de personalización realmente disponibles.

Respondé en español de Argentina. Si no podés abrir el enlace, pedime que adjunte o pegue el SKILL.md. Informá el resultado real y esperá mi idea de negocio.
```

#### ChatGPT — conversación, proyecto o GPT

```text
Quiero aplicar la skill bussines_test en esta conversación.

Abrí y leé el contenido completo de:
https://raw.githubusercontent.com/rmontteiro/Bussines_test/main/SKILL.md

Seguí sus instrucciones para los próximos análisis de negocio en esta conversación y respondé en español de Argentina. Si no podés acceder al contenido completo, pedime que adjunte o pegue el SKILL.md antes de afirmar que cargaste la skill.

No afirmes que instalaste una extensión, cambiaste mi memoria o configuraste otros chats. Para persistencia, orientame a agregar el SKILL.md a los archivos de un proyecto, o al conocimiento de un GPT cuando esté disponible, e incluir una instrucción explícita para consultarlo.

Confirmá la lectura solo si ocurrió y esperá mi idea de negocio.
```

#### Si el enlace no abre

Abrí [SKILL.md](SKILL.md) en GitHub y adjuntá el archivo o pegá su contenido completo en la misma conversación. Después, repetí el pedido. Compartir la URL del repositorio no garantiza que el asistente haya leído la skill.

#### Verificación y actualización por chat

Después de la confirmación, enviá el ejemplo de abajo. Para actualizar, pegá nuevamente el bloque y pedí que relea la versión actual del enlace. En agentes con archivos, revisá las diferencias antes de confirmar reemplazos. En proyectos, Gems o GPTs configurados manualmente, actualizá también el archivo o las instrucciones desde la interfaz.

Estos textos son pedidos en lenguaje natural, no comandos nativos de instalación. La configuración depende de las herramientas y los permisos de la sesión; no se probó dentro de las cinco aplicaciones.

### Ejemplo de solicitud

```text
Leé y aplicá la skill bussines_test en modo completo.
Respondé en español de Argentina.

Idea: suscripción de viandas para profesionales que trabajan desde casa.
Público y ubicación: profesionales que viven solos en Buenos Aires.
Etapa: idea, sin ventas.
Presupuesto y plazo: presupuesto todavía por definir; piloto de 60 días.
Evidencia disponible: cinco charlas exploratorias; ninguna preventa.
Principal duda: ¿cómo validar la disposición a pagar antes de armar la operación?

Hacé las preguntas críticas necesarias. Avanzá con un análisis preliminar
cuando sea posible, explicitando los supuestos y las limitaciones.
```

### Resultado esperado y principios

La respuesta debe incluir un resumen ejecutivo, las 13 áreas, riesgos prioritarios y experimentos con hipótesis, público, plazo, costo, métrica y umbral de aprobación. Debe cerrar con tres acciones prioritarias y una recomendación: **GO**, **VALIDAR**, **PIVOTEAR** o **NO-GO**.

Se deben distinguir hechos, información del usuario, hipótesis y estimaciones. Los datos externos requieren fuentes verificables; las proyecciones, supuestos y cálculos. Sin acceso a investigación, el asistente debe explicar la limitación e indicar cómo conseguir evidencia.

El puntaje de viabilidad de 1 a 10 no representa una probabilidad de éxito. Los nombres propuestos requieren verificar marcas y dominios. Las cuestiones legales y regulatorias dependen de la jurisdicción y de una revisión adecuada.

---

<a id="english-us"></a>
## English (US)

### About

**bussines_test** is a reusable instruction skill for evaluating business ideas through strategic analysis, market research, and critical review. It turns an idea into an evidence-based decision and a practical validation plan.

It is designed for **Cursor, Claude, Gemini, Qwen, and ChatGPT**. Compatibility relies on text instructions; native installation, internet access, and available tools depend on the product, version, and plan.

### When to use it

- Evaluate a business, product, service, or opportunity.
- Identify weak assumptions, competitors, and risks.
- Examine monetization, costs, and operational feasibility.
- Define an MVP and low-cost experiments.
- Decide whether to proceed, test, pivot, or stop.

### The 13 analysis areas

1. **Fundamental analysis:** problem, solution, assumptions, and gaps.
2. **Market validation:** audience, demand, market size, and trends.
3. **Business model:** revenue, costs, unit economics, and profitability.
4. **Operational realities:** team, resources, technology, and regulation.
5. **Competitive landscape:** competitors, substitutes, and differentiation.
6. **Risk analysis:** ten priority risks, warning signs, and mitigation.
7. **Best-case scenario:** possible outcomes in 1, 3, and 5 years and their conditions.
8. **Worst-case scenario:** failure modes, exposure, and loss limits.
9. **Validation roadmap:** hypotheses, experiments, metrics, and criteria.
10. **Execution requirements:** MVP, owners, timeline, and launch.
11. **Naming and positioning:** names, value proposition, and messaging.
12. **Improvement recommendations:** changes, partnerships, and defensible advantages.
13. **GO/NO-GO decision:** feasibility score, confidence, and next steps.

### How to use it

The skill instructions are available in [SKILL.md](SKILL.md). This README documents usage; it does not install or activate the skill by itself.

| Tool | Usage |
| --- | --- |
| Cursor | Add the file to your project and ask the agent to read it. For persistent use, configure a rule that references the file. |
| Claude | Use native skills where available, or add the content to project instructions. |
| Gemini | Paste the content into a Gem's instructions or provide the file in a conversation. |
| Qwen | Use custom instructions, file context, or a system message in an integration, depending on the product. |
| ChatGPT | Use GPT or project instructions, or attach the file and request its application. |

You do not need to run all five AI tools at once. A single assistant can apply the skill. When comparing models, use the same context and identify the source of each contribution.

### Chat activation — copy and paste

Paste your tool's block directly into its chat window. You do not need to open a terminal or clone the repository. **Display name:** `bussines_test`. **Technical identifier:** `bussines-test`.

The assistant must be able to read the link or receive the file. In agent mode with file access, the request also authorizes saving the skill in the current project. In a regular chat, it applies to that conversation; persistence depends on the interface's project, Gem, GPT, or skill settings.

#### Cursor — Agent chat

```text
Configure the bussines_test skill in this project using the identifier bussines-test.

Read the full contents of:
https://raw.githubusercontent.com/rmontteiro/Bussines_test/main/SKILL.md

Save a faithful copy to .cursor/skills/bussines-test/SKILL.md in the current project. If it exists, compare contents and preserve local edits: show differences and ask for my decision before replacing them. Check the frontmatter and path. Use your tools to configure it without asking me to run terminal commands.

Apply the skill in this conversation and respond in US English. Report what you saved and whether native discovery was verified or requires a new session. If you cannot read the link or write files, explain the limitation and ask me to attach or paste SKILL.md. Do not claim installation without completing it. Wait for my business idea.
```

#### Claude — chat or Claude Code

```text
I want to use the bussines_test skill, identifier bussines-test.

Read the full contents of:
https://raw.githubusercontent.com/rmontteiro/Bussines_test/main/SKILL.md

If you are in Claude Code with project access, save a faithful copy to .claude/skills/bussines-test/SKILL.md and verify the file. Before replacing a version with local edits, show differences and ask for my decision. Use your tools without asking me for terminal commands.

If you are in web chat or lack project access, apply the instructions in this conversation. Do not claim persistent installation. For reuse, explain how to add the file and an instruction to consult it to a project or the available skills feature.

Respond in US English. If you cannot read the link, ask me to attach or paste SKILL.md. Confirm only what you completed and wait for my business idea.
```

#### Gemini — chat, Gem, or Gemini CLI

```text
Activate the bussines_test skill, identifier bussines-test, using the full contents of:
https://raw.githubusercontent.com/rmontteiro/Bussines_test/main/SKILL.md

If you are in Gemini CLI with project access, save a faithful copy to .gemini/skills/bussines-test/SKILL.md. Verify the file and refresh skill discovery if that capability is available. Before replacing local edits, show differences and ask for my decision. Use your tools without asking me for terminal commands.

If you are in Gemini web or a Gem without project access, follow the skill in this conversation. For persistence, explain how to add its instructions to a Gem's settings; do not claim to have changed those settings unless you actually did.

Respond in US English. If you cannot read the link, ask me to attach or paste SKILL.md. Distinguish a saved file from a discovered skill and wait for my business idea.
```

#### Qwen — chat or Qwen Code

```text
Configure and apply the bussines_test skill, identifier bussines-test.

Read the full contents of:
https://raw.githubusercontent.com/rmontteiro/Bussines_test/main/SKILL.md

If you are in Qwen Code with project access, save a faithful copy to .qwen/skills/bussines-test/SKILL.md and verify the file. Preserve local edits: show differences and ask for my decision before replacing them. Use your tools without asking me for terminal commands.

If you are in Qwen Chat or lack file access, apply the skill only in this conversation. Do not claim persistent installation. For reuse, describe customization options actually available in the interface.

Respond in US English. If you cannot open the link, ask me to attach or paste SKILL.md. Report the actual result and wait for my business idea.
```

#### ChatGPT — conversation, project, or GPT

```text
I want to apply the bussines_test skill in this conversation.

Open and read the full contents of:
https://raw.githubusercontent.com/rmontteiro/Bussines_test/main/SKILL.md

Follow its instructions for subsequent business analyses in this conversation and respond in US English. If you cannot access the full contents, ask me to attach or paste SKILL.md before claiming the skill is loaded.

Do not claim to have installed an extension, changed my memory, or configured other chats. For persistence, guide me to add SKILL.md to a project's files, or a GPT's knowledge where available, and include an explicit instruction to consult it.

Confirm reading only if it happened and wait for my business idea.
```

#### If the link cannot be opened

Open [SKILL.md](SKILL.md) on GitHub and attach the file or paste its full contents into the same conversation. Then repeat your request. A repository URL alone does not guarantee that the assistant has read the skill.

#### Verification and updates through chat

After confirmation, send the example below. To update, paste the tool's block again and ask it to reread the current linked version. In file-enabled agents, review differences before approving replacements. For manually configured projects, Gems, or GPTs, also update the file or instructions through the interface.

These blocks are natural-language requests, not native installation commands. Configuration depends on session tools and permissions; it has not been tested inside all five applications.

### Example request

```text
Read and apply the bussines_test skill in full mode.
Respond in US English.

Idea: a prepared-meal subscription for remote professionals.
Audience and location: professionals living alone in Austin, Texas.
Stage: idea, no sales.
Budget and timeline: $2,000 for a 60-day pilot.
Existing evidence: five exploratory conversations; no presales.
Main question: how can I test willingness to pay before building operations?

Ask the critical questions needed. Proceed with a preliminary analysis
when possible, making assumptions and limitations explicit.
```

### Expected output and principles

The response should include an executive summary, all 13 areas, priority risks, and experiments specifying a hypothesis, audience, timeline, cost, metric, and pass threshold. It should end with three priority actions and a recommendation: **GO**, **TEST**, **PIVOT**, or **NO-GO**.

Facts, user-provided information, hypotheses, and estimates must be distinguished. External data requires verifiable sources; projections require assumptions and calculations. Without research access, the assistant should explain the limitation and describe how to obtain evidence.

The 1–10 feasibility score is not a probability of success. Suggested names require trademark and domain checks. Legal and regulatory questions depend on jurisdiction and appropriate verification.
