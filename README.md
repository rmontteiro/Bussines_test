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

### Instalação

O arquivo [SKILL.md](SKILL.md) está incluído no repositório. **Nome de apresentação:** `bussines_test`. **Identificador de instalação e comando:** `bussines-test`, com hífen para compatibilidade com o formato Agent Skills.

#### 1. Baixar o repositório

Pré-requisitos: Git e a ferramenta de destino já instalada e autenticada. Os comandos abaixo usam Bash (macOS, Linux ou Git Bash no Windows). Execute o clone apenas na primeira instalação; se já tiver uma cópia, entre nela e use `git pull --ff-only`.

```bash
git clone https://github.com/rmontteiro/Bussines_test.git
cd Bussines_test
```

#### 2. Instalar na ferramenta

Os blocos de cópia abaixo instalam no escopo pessoal, para uso entre projetos. Execute-os a partir da pasta clonada. `cp -i` pede confirmação antes de substituir um arquivo existente.

#### Cursor

```bash
mkdir -p "$HOME/.cursor/skills/bussines-test"
cp -i SKILL.md "$HOME/.cursor/skills/bussines-test/SKILL.md"
```

Depois, abra uma nova conversa no Agent e peça para aplicar `bussines-test`.

#### Claude Code

```bash
mkdir -p "$HOME/.claude/skills/bussines-test"
cp -i SKILL.md "$HOME/.claude/skills/bussines-test/SKILL.md"
```

Abra uma sessão do Claude Code e invoque:

```text
/bussines-test
```

#### Gemini CLI

O Gemini CLI pode instalar diretamente do GitHub. Confirme a instalação quando solicitado. Para instalar somente no projeto atual, substitua `--scope user` por `--scope workspace`.

```bash
gemini skills install https://github.com/rmontteiro/Bussines_test.git --scope user
gemini skills list
```

#### Qwen Code

```bash
mkdir -p "$HOME/.qwen/skills/bussines-test"
cp -i SKILL.md "$HOME/.qwen/skills/bussines-test/SKILL.md"
```

Abra uma nova sessão do Qwen Code, consulte `/skills` e peça para aplicar `bussines-test`.

#### ChatGPT e interfaces web

**ChatGPT:** os comandos anteriores não instalam uma skill no ChatGPT. Abra um projeto, adicione `SKILL.md` aos arquivos e inclua nas instruções: “Antes de avaliar ideias de negócio, leia e aplique o arquivo SKILL.md; responda em português do Brasil”. Para um GPT personalizado, quando disponível, adicione o arquivo ao conhecimento e uma instrução explícita para consultá-lo. Em uma conversa avulsa, anexe o arquivo e peça sua aplicação.

**Claude web, Gemini web e Qwen Chat:** use o conteúdo do arquivo nas instruções de projeto, personalização ou Gem quando o produto oferecer esse recurso; alternativamente, anexe ou cole o conteúdo na conversa e peça para segui-lo. A instalação no Claude Code, Gemini CLI ou Qwen Code não configura automaticamente as respectivas interfaces web.

#### Alternativa no Windows PowerShell

Na pasta clonada, escolha o destino na tabela e execute o bloco. Use somente uma linha de atribuição a `$skillTarget` por instalação.

| Tool | PowerShell |
| --- | --- |
| Cursor | `$skillTarget = Join-Path $HOME '.cursor/skills/bussines-test'` |
| Claude Code | `$skillTarget = Join-Path $HOME '.claude/skills/bussines-test'` |
| Qwen Code | `$skillTarget = Join-Path $HOME '.qwen/skills/bussines-test'` |

```powershell
New-Item -ItemType Directory -Force -Path $skillTarget | Out-Null
Copy-Item -LiteralPath .\SKILL.md -Destination (Join-Path $skillTarget 'SKILL.md') -Confirm
```

#### Verificação e atualização

Verifique se `bussines-test` aparece na lista de skills da ferramenta e peça uma análise curta de uma ideia. Se não aparecer, confira o caminho e abra uma nova sessão. Para atualizar, rode `git pull --ff-only` na cópia do repositório e repita a cópia para a ferramenta. No Gemini CLI, se a versão já instalada impedir reinstalação, remova-a com `gemini skills uninstall bussines-test --scope user` e repita o comando de instalação.

Os comandos foram conferidos com a documentação oficial; a ativação em cada aplicativo depende da versão e não foi testada nesta sessão. Instalar os arquivos não exige chaves de API específicas desta skill.

Documentação oficial: [Cursor](https://cursor.com/docs/skills) · [Claude Code](https://code.claude.com/docs/en/skills) · [Gemini CLI](https://geminicli.com/docs/cli/skills/) · [Qwen Code](https://qwenlm.github.io/qwen-code-docs/en/users/features/skills/) · [ChatGPT Projects](https://help.openai.com/en/articles/10169521-projects-in-chatgpt) · [GPTs](https://help.openai.com/en/articles/8554397-creating-and-editing-gpts)

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

### Instalación

El archivo [SKILL.md](SKILL.md) está incluido en el repositorio. **Nombre visible:** `bussines_test`. **Identificador de instalación y comando:** `bussines-test`, con guion para respetar el formato Agent Skills.

#### 1. Descargar el repositorio

Requisitos: Git y la herramienta de destino ya instalada y autenticada. Los comandos usan Bash (macOS, Linux o Git Bash en Windows). Cloná una sola vez; si ya tenés una copia, entrá en esa carpeta y ejecutá `git pull --ff-only`.

```bash
git clone https://github.com/rmontteiro/Bussines_test.git
cd Bussines_test
```

#### 2. Instalar en la herramienta

Los bloques de copia instalan la skill en el ámbito personal, para todos tus proyectos. Ejecutalos desde la carpeta clonada. `cp -i` pide confirmación antes de reemplazar un archivo existente.

#### Cursor

```bash
mkdir -p "$HOME/.cursor/skills/bussines-test"
cp -i SKILL.md "$HOME/.cursor/skills/bussines-test/SKILL.md"
```

Después, abrí una conversación nueva en Agent y pedile que aplique `bussines-test`.

#### Claude Code

```bash
mkdir -p "$HOME/.claude/skills/bussines-test"
cp -i SKILL.md "$HOME/.claude/skills/bussines-test/SKILL.md"
```

Abrí una sesión de Claude Code e invocá:

```text
/bussines-test
```

#### Gemini CLI

Gemini CLI permite instalar directamente desde GitHub. Confirmá la instalación cuando te lo pida. Para instalar solo en el proyecto actual, reemplazá `--scope user` por `--scope workspace`.

```bash
gemini skills install https://github.com/rmontteiro/Bussines_test.git --scope user
gemini skills list
```

#### Qwen Code

```bash
mkdir -p "$HOME/.qwen/skills/bussines-test"
cp -i SKILL.md "$HOME/.qwen/skills/bussines-test/SKILL.md"
```

Abrí una sesión nueva de Qwen Code, consultá `/skills` y pedile que aplique `bussines-test`.

#### ChatGPT e interfaces web

**ChatGPT:** los comandos anteriores no instalan una skill en ChatGPT. Creá un proyecto, agregá `SKILL.md` a los archivos e incluí esta instrucción: “Antes de evaluar ideas de negocio, leé y aplicá SKILL.md; respondé en español de Argentina”. Para un GPT personalizado, cuando esté disponible, agregá el archivo al conocimiento y una instrucción explícita para consultarlo. En un chat suelto, adjuntá el archivo y pedí su aplicación.

**Claude web, Gemini web y Qwen Chat:** usá el contenido en las instrucciones de un proyecto, la personalización o un Gem cuando el producto lo permita; también podés adjuntarlo o pegarlo en la conversación y pedir que lo siga. Instalar en Claude Code, Gemini CLI o Qwen Code no configura automáticamente las interfaces web.

#### Alternativa en Windows PowerShell

Desde la carpeta clonada, elegí el destino de la tabla y ejecutá el bloque. Usá una sola asignación a `$skillTarget` por instalación.

| Tool | PowerShell |
| --- | --- |
| Cursor | `$skillTarget = Join-Path $HOME '.cursor/skills/bussines-test'` |
| Claude Code | `$skillTarget = Join-Path $HOME '.claude/skills/bussines-test'` |
| Qwen Code | `$skillTarget = Join-Path $HOME '.qwen/skills/bussines-test'` |

```powershell
New-Item -ItemType Directory -Force -Path $skillTarget | Out-Null
Copy-Item -LiteralPath .\SKILL.md -Destination (Join-Path $skillTarget 'SKILL.md') -Confirm
```

#### Verificación y actualización

Verificá que `bussines-test` aparezca en la lista de skills y pedí un análisis breve. Si no aparece, revisá la ruta y abrí una sesión nueva. Para actualizar, ejecutá `git pull --ff-only` en la copia del repositorio y repetí la copia. En Gemini CLI, si la versión instalada impide reinstalar, ejecutá `gemini skills uninstall bussines-test --scope user` y repetí la instalación.

Los comandos se contrastaron con la documentación oficial; la activación depende de la versión y no se probó dentro de cada aplicación en esta sesión. Esta skill no requiere claves de API propias para instalar sus archivos.

Documentación oficial: [Cursor](https://cursor.com/docs/skills) · [Claude Code](https://code.claude.com/docs/en/skills) · [Gemini CLI](https://geminicli.com/docs/cli/skills/) · [Qwen Code](https://qwenlm.github.io/qwen-code-docs/en/users/features/skills/) · [ChatGPT Projects](https://help.openai.com/en/articles/10169521-projects-in-chatgpt) · [GPTs](https://help.openai.com/en/articles/8554397-creating-and-editing-gpts)

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

### Installation

The repository includes [SKILL.md](SKILL.md). **Display name:** `bussines_test`. **Installation identifier and command:** `bussines-test`, using a hyphen for Agent Skills compatibility.

#### 1. Download the repository

Prerequisites: Git and an installed, authenticated target tool. Commands use Bash (macOS, Linux, or Git Bash on Windows). Clone only once; if you already have a copy, open that folder and run `git pull --ff-only`.

```bash
git clone https://github.com/rmontteiro/Bussines_test.git
cd Bussines_test
```

#### 2. Install in your tool

The copy blocks install a personal skill across projects. Run them from the cloned folder. `cp -i` asks before replacing an existing file.

#### Cursor

```bash
mkdir -p "$HOME/.cursor/skills/bussines-test"
cp -i SKILL.md "$HOME/.cursor/skills/bussines-test/SKILL.md"
```

Then open a new Agent conversation and ask it to apply `bussines-test`.

#### Claude Code

```bash
mkdir -p "$HOME/.claude/skills/bussines-test"
cp -i SKILL.md "$HOME/.claude/skills/bussines-test/SKILL.md"
```

Open a Claude Code session and invoke:

```text
/bussines-test
```

#### Gemini CLI

Gemini CLI supports installation directly from GitHub. Confirm installation when prompted. For the current project only, replace `--scope user` with `--scope workspace`.

```bash
gemini skills install https://github.com/rmontteiro/Bussines_test.git --scope user
gemini skills list
```

#### Qwen Code

```bash
mkdir -p "$HOME/.qwen/skills/bussines-test"
cp -i SKILL.md "$HOME/.qwen/skills/bussines-test/SKILL.md"
```

Open a new Qwen Code session, check `/skills`, and ask it to apply `bussines-test`.

#### ChatGPT and web interfaces

**ChatGPT:** the commands above do not install a skill into ChatGPT. Create a project, add `SKILL.md` to its files, and add this instruction: “Before evaluating business ideas, read and apply SKILL.md; respond in US English.” For a custom GPT, where available, add the file as knowledge and explicitly instruct the GPT to consult it. For a standalone chat, attach the file and ask the assistant to apply it.

**Claude web, Gemini web, and Qwen Chat:** use the content in project instructions, customization, or a Gem where supported; alternatively, attach or paste it into a conversation and ask the assistant to follow it. Installing into Claude Code, Gemini CLI, or Qwen Code does not automatically configure the corresponding web interface.

#### Windows PowerShell alternative

From the cloned folder, choose a target from the table and run the block. Use only one `$skillTarget` assignment per installation.

| Tool | PowerShell |
| --- | --- |
| Cursor | `$skillTarget = Join-Path $HOME '.cursor/skills/bussines-test'` |
| Claude Code | `$skillTarget = Join-Path $HOME '.claude/skills/bussines-test'` |
| Qwen Code | `$skillTarget = Join-Path $HOME '.qwen/skills/bussines-test'` |

```powershell
New-Item -ItemType Directory -Force -Path $skillTarget | Out-Null
Copy-Item -LiteralPath .\SKILL.md -Destination (Join-Path $skillTarget 'SKILL.md') -Confirm
```

#### Verification and updates

Check that `bussines-test` appears in the tool's skill list and request a short business analysis. If it is missing, check the path and start a new session. To update, run `git pull --ff-only` in the repository copy and repeat the copy step. In Gemini CLI, if the installed version prevents reinstallation, run `gemini skills uninstall bussines-test --scope user` and repeat installation.

Commands were checked against official documentation; activation depends on the application version and was not tested inside each application in this session. No skill-specific API keys are required to install these files.

Official documentation: [Cursor](https://cursor.com/docs/skills) · [Claude Code](https://code.claude.com/docs/en/skills) · [Gemini CLI](https://geminicli.com/docs/cli/skills/) · [Qwen Code](https://qwenlm.github.io/qwen-code-docs/en/users/features/skills/) · [ChatGPT Projects](https://help.openai.com/en/articles/10169521-projects-in-chatgpt) · [GPTs](https://help.openai.com/en/articles/8554397-creating-and-editing-gpts)

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
