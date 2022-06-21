# Jobs
- Um Build contém um ou mais Jobs. A maioria dos Jobs é de um agente. 
  Um Job representa um limite de execução de um conjunto de Steps. Todos os steps correm juntos com o mesmo agente.
  Por exemplo, você pode construir duas configurações - x86 e x64. Neste caso, você tem um build e dois jobs.

## Tipos de Jobs
No Azure DevOps, existem quatro tipos de vagas disponíveis:
- Agent pool Jobs
- Container Jobs
- Deployment group jobs
- Agentless jobs

### Agent pool Jobs
- Os tipos mais comuns de Job. Os Jobs são executados em um agente que faz parte de um grupo de agentes(Agent Pool).

-Em vez de gerenciar cada agente individualmente, você organiza agentes em grupos de agentes. Um grupo de agentes define o limite de compartilhamento para todos os agentes naquele pool.
No Azure Pipelines, os pools são um escopo para toda a organização para que você possa compartilhar as máquinas de agentes através de projetos.
Se você criar um pool de agentes para um projeto específico, somente esse projeto pode usar o pool até adicionar o pool de projetos em outro projeto.
Ao criar um pipeline de build ou release, você pode especificar qual pool ele usa, organização ou escopo de projeto.
Pools escopo para um projeto só podem usá-los através do build e release de Pipelines dentro de um projeto.
Para compartilhar um pool de agentes com vários projetos, use um pool de agentes de escopo de organização e adicione-os em cada um desses projetos, adicione um pool de agentes existente e escolha o pool de agentes da organização. Se você criar um novo pool de agentes, você pode conceder automaticamente permissão de acesso a todos os pipelines.

### Container jobs
- Jobs semelhantes ao Agent Pool Jobs, executados em um contêiner em uma parte agente de um Agent Pool.

### Deployment group jobs
- Jobs que funcionam em sistemas em um grupo de implantação(Deployment Group).

### Agentless jobs
- Jobs que funcionam diretamente no Azure DevOps. Eles não precisam de um agente para execução. Também é muitas vezes chamado de **Server Jobs**‎
