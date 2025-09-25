# resumo-do-lab.
Este repositório contém o resumo das lições aprendidas durante o desenvolvimento do lab na DIO

Resumo da Introdução e serviços Descristos até o momento 
 Conceitos fundamentais de computação em nuvem

Definição: Nuvem é a entrega de recursos de TI (computação, armazenamento, rede, serviços) sob demanda via internet, com cobrança baseada em uso.
Modelos de implantação:
Nuvem Pública: Recursos gerenciados por provedores (ex.: Azure). Alta escala e custo inicial baixo.
Nuvem Privada: Infraestrutura dedicada a uma organização (on-premises ou hosted). Maior controle e custo.
Nuvem Híbrida: Integração entre nuvem pública e privada para balancear controle, custo e segurança.

Modelos de Serviço:
IaaS (Infrastructure as a Service): VMs, redes, discos — você gerencia SO e aplicações. Ex.: Azure Virtual Machines.
PaaS (Platform as a Service): Plataforma gerenciada (runtime, middleware). Reduz responsabilidade operacional. Ex.: Azure App Service.
SaaS (Software as a Service): Aplicações prontas para uso fornecidas pelo provedor. Ex.: Microsoft 365.

 Principais benefícios da nuvem
Elasticidade e escalabilidade: ajustar recursos conforme demanda (scale up/down, scale out/in).
Pagamento por uso: redução de investimento inicial.
Alta disponibilidade e recuperação: múltiplas regiões/zonas para tolerância a falhas e DR.
Agilidade e inovação: provisionamento rápido de recursos.

 CapEx vs OpEx
CapEx (Capital Expenditure): investimento em hardware e data center (capex alto, depreciação).
OpEx (Operational Expenditure): despesas operacionais com serviços consumidos (modelo de nuvem típico).
Implicação prática: migrar para nuvem tende a transformar CapEx em OpEx e permitir escalabilidade e elasticidade.

 Serviços centrais do Azure (visão prática para prova)
Compute
Virtual Machines (VMs): IaaS, controle total do SO; escalabilidade manual/auto-scale com conjuntos de dimensionamento (VM Scale Sets).
App Service: PaaS para hospedar aplicações web e APIs; gerenciamento de plataforma.
Azure Functions: computação serverless — execução por evento, cobrança por execução.
Azure Kubernetes Service (AKS): orquestração de contêineres com Kubernetes; reduz overhead operacional.

Storage
Blob Storage: objetos/arquivos não-estruturados (arquivos, backups, logs).
File Storage: compartilhamento de arquivos gerenciado (SMB).
Disk Storage: discos gerenciados para VMs.
Queue/Table: serviços de mensagem e armazenamento NoSQL simples.

Networking
Virtual Network (VNet): rede lógica isolada para recursos do Azure.
Subnets, NSG (Network Security Group): segmentação e regras de filtragem.
Load Balancer / Application Gateway: balanceamento de tráfego; Application Gateway oferece WAF.
VPN Gateway / ExpressRoute: conectividade segura entre on-premises e Azure (ExpressRoute = link privado dedicado).

Bancos de dados
Azure SQL Database: banco relacional PaaS.
Cosmos DB: banco NoSQL multimodel, replicação global, latência baixa.
Identidade e segurança
Azure Active Directory (Azure AD): identidade e gestão de acesso (SSO, MFA, gerenciamento de usuários).
RBAC (Role-Based Access Control): permissões por função aplicadas a recursos.
Key Vault: gerenciamento de chaves, segredos e certificados.
Azure Defender / Microsoft Defender for Cloud: proteção contra ameaças.
Azure Firewall / NSG / WAF: controles de rede e proteção de aplicações.

Observabilidade e gerenciamento
Azure Monitor: coleta de métricas, logs e alertas.
Azure Advisor: recomendações para otimização de custos, desempenho e segurança.
Azure Policy e Blueprints: governança e conformidade automatizada.
Subscriptions, Resource Groups, Management Groups: organização e limites administrativos.
Preço e SLA
Modelos de cobrança: pay-as-you-go, reservas (discounts for reserved capacity), custo por recurso/segundo/hora.
SLA: acordos de disponibilidade que variam por serviço; entender o impacto na arquitetura (redundância entre zonas/regiões).
Cost Management: monitoramento e otimização de custos.

 Azure AI — tópicos relevantes para AZ-900

Visão geral: Azure oferece um conjunto de serviços que facilitam a incorporação de capacidades de IA sem necessidade de criar toda a infraestrutura ou modelos do zero. Para AZ-900, foque em reconhecer o propósito e o uso de cada serviço, não em detalhes avançados de implementação.
Serviços principais e o que cai na prova (nível fundamental)
Azure Cognitive Services: APIs pré-treinadas para visão (Computer Vision), fala (Speech), linguagem (Text Analytics, Translator) e tomada de decisão.
Ponto de prova: saber que são APIs gerenciadas para adicionar capacidades de IA (ex.: análise de texto, extração de entidades, OCR).
Azure OpenAI Service: serviço gerenciado que disponibiliza modelos de linguagem (ex.: GPT) para geração de texto, resumo, embeddings e similaridade.
Ponto de prova: entender o propósito (modelos de linguagem prontos), casos de uso (chatbots, geração de conteúdo, embeddings) e preocupações (privacidade dos dados, responsabilidade e governança).
Observação prática: políticas de uso e considerações de conformidade e segurança são importantes; detalhes operacionais (como processos de aprovação ou quotas) podem variar ao longo do tempo.
Azure Machine Learning: plataforma para treinar, implantar e gerenciar modelos; suporta MLOps e ciclo de vida de modelos.
Ponto de prova: conceito básico de que é a ferramenta para desenvolvimento e operação de modelos personalizados.
Casos de uso comuns (nível exame): reconhecimento de imagem, transcrição de fala, análise de sentimento, tradução automática, chatbots, análise de documentos, auxílio à tomada de decisão.
Considerações de segurança e conformidade (Azure AI)
Proteção de dados (armazenamento seguro, criptografia, Key Vault).
Práticas de Responsible AI (mitigar vieses, monitorar resultados).
Necessidade de verificar requisitos de conformidade e região para dados sensíveis.

 Revisão por domínio (resumo rápido)
Computação em nuvem: benefícios e modelos (IaaS/PaaS/SaaS).
Modelos de implantação: pública, privada, híbrida.
CapEx vs OpEx: diferença e impacto financeiro.
Serviços Azure principais: compute, storage, networking, identity, banco de dados.
Segurança e identidade: Azure AD, RBAC, MFA, Key Vault.
Governança: subscriptions, resource groups, Azure Policy, cost management.
Observabilidade: Azure Monitor, logs, alertas.
IA no Azure: Cognitive Services, Azure OpenAI Service, Azure Machine Learning.
Preço e suporte: modelos de cobrança, SLAs, planos de suporte.

