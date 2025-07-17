# Auditoria de Segurança e Conformidade: Estudo de Caso da Botium Toys

## 1. Resumo do Projeto

Este repositório contém os artefatos e a análise de uma auditoria de segurança da informação realizada na empresa fictícia Botium Toys. O objetivo foi avaliar a postura de segurança da empresa, identificar vulnerabilidades, verificar a conformidade com padrões relevantes e fornecer recomendações para mitigar os riscos encontrados.

---

## 2. Contexto e Objetivos

### Escopo
O escopo da auditoria foi definido como todo o programa de segurança da Botium Toys. Isso significa que todos os ativos, processos e procedimentos internos relacionados à implementação de controles e conformidade foram avaliados. Os ativos incluem:
* Equipamento local para necessidades de negócios no escritório.
* Equipamentos de funcionários, como dispositivos de usuário final (desktops/laptops, smartphones), estações de trabalho remotas, fones de ouvido, entre outros.
* Produtos de vitrine disponíveis para venda, armazenados no depósito.
* Sistemas de gestão, software e serviços para contabilidade, telecomunicações, banco de dados, segurança, comércio eletrônico e gestão de estoque.
* Acesso à Internet e a rede interna.
* Sistemas de retenção e armazenamento de dados.
* Sistemas legados em fim de vida útil que requerem monitoramento humano.

### Objetivos
O principal objetivo foi avaliar os ativos existentes e preencher a lista de verificação de controles e conformidade para determinar as ações necessárias para fortalecer a segurança da Botium Toys.

---

## 3. Avaliação de Risco e Principais Descobertas

A avaliação inicial identificou uma **pontuação de risco de 8 em 10**, considerada alta. Esse risco elevado deve-se à falta de controles adequados e à não adesão às melhores práticas de conformidade.

### Descobertas Críticas:
* **Gestão de Acesso Inadequada**: Atualmente, todos os funcionários da Botium Toys têm acesso a dados armazenados internamente, incluindo dados de titulares de cartão e PII/SPII dos clientes. Controles de acesso baseados no princípio do privilégio mínimo e na separação de tarefas não foram implementados.
* **Falta de Criptografia**: A criptografia não é utilizada para proteger as informações de cartão de crédito dos clientes que são aceitas, processadas, transmitidas e armazenadas internamente.
* **Ausência de Recuperação de Desastres**: A empresa não possui planos de recuperação de desastres. Adicionalmente, não são feitos backups de dados críticos.
* **Políticas de Senha Fracas**: Embora exista uma política de senha, seus requisitos são nominais e não estão alinhados com os padrões atuais de complexidade. Não há um sistema de gerenciamento de senhas centralizado para impor tais requisitos.
* **Falta de Detecção de Intrusão**: A empresa não instalou um sistema de detecção de intrusão (IDS).
* **Sistemas Leg
