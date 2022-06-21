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

### Container jobs
- Jobs semelhantes ao Agent Pool Jobs, executados em um contêiner em uma parte agente de um Agent Pool.

### Deployment group jobs
- Jobs que funcionam em sistemas em um grupo de implantação(Deployment Group).

### Agentless jobs
- Jobs que funcionam diretamente no Azure DevOps. Eles não precisam de um agente para execução. Também é muitas vezes chamado de **Server Jobs**‎
