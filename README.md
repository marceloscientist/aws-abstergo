# Relatório de implementação de serviços AWS
Data: 2025-05-13
Empresa: Abstergo Industries
Responsável: Marcelo Silva

## Introdução
Este relatório apresenta o processo de implementação de ferramentas na empresa Abstergo Industries, realizado por Marcelo. O objetivo do projeto foi elencar 3 serviços AWS, com a finalidade de realizar diminuição de custos imediatos.

## Descrição do Projeto
O projeto de implementação de ferramentas foi dividido em 3 etapas, cada uma com seus objetivos específicos. A seguir, serão descritas as etapas do projeto:

### Etapa 1:
Nome da ferramenta: AWS S3 (Simple Storage Service)

Foco da ferramenta: Armazenamento seguro e escalável de arquivos e backups

Descrição do caso de uso:
Abstergo utilizava servidores locais para armazenar documentos e imagens de produtos. Com a migração para o Amazon S3, todos os dados de marketing, etiquetas de produtos e contratos foram transferidos para buckets com políticas de versionamento e ciclo de vida. Isso reduziu drasticamente o custo com infraestrutura física e aumentou a confiabilidade dos backups.

### Etapa 2:
Nome da ferramenta: AWS Lambda

Foco da ferramenta: Execução de código sob demanda sem necessidade de servidores

Descrição do caso de uso:
Automatizou-se a geração de relatórios de estoque e faturamento com funções Lambda ativadas por eventos no S3. Sempre que um arquivo CSV era salvo no bucket, a função Lambda processava os dados e gerava relatórios no formato PDF, economizando com servidores EC2 que eram mantidos ativos apenas para isso.

### Etapa 3:
Nome da ferramenta: AWS CloudWatch + Auto Scaling

Foco da ferramenta: Monitoramento de performance e escalabilidade automática

Descrição do caso de uso:
O ambiente de aplicação da Abstergo foi configurado com CloudWatch para monitorar o uso de CPU e memória, integrando com grupos de Auto Scaling. Dessa forma, as instâncias EC2 sobem ou descem automaticamente conforme a demanda, evitando custos com recursos ociosos.

## Conclusão
A implementação de ferramentas na empresa Abstergo Industries tem como esperado reduzir custos com infraestrutura, aumentar a eficiência operacional e automatizar tarefas repetitivas, o que aumentará a eficiência e a produtividade da empresa. Recomenda-se a continuidade da utilização das ferramentas implementadas e a busca por novas tecnologias que possam melhorar ainda mais os processos da empresa.
