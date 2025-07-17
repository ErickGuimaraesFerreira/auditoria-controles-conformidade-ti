# Auditoria de Segurança e Conformidade: Estudo de Caso da Botium Toys

## 1. Resumo do Projeto

Este repositório contém os artefatos e a análise de uma auditoria de segurança da informação realizada na empresa fictícia Botium Toys. O objetivo foi avaliar a postura de segurança da empresa, identificar vulnerabilidades, verificar a conformidade com padrões relevantes e fornecer recomendações para mitigar os riscos encontrados.

---

## 2. Contexto e Objetivos

### Escopo
O escopo da auditoria foi definido como todo o programa de segurança da Botium Toys. Isso significa que todos os ativos, processos e procedimentos internos relacionados à implementação de controles e conformidade foram avaliados. Os ativos incluem:
* Equipamento local para necessidades de negócios no escritório.
* Equipamentos de funcionários, como dispositivos de usuário final (desktops/laptops, smartphones), estações de trabalho remotas, fones de ouvido, entre outros.
* Produtos de vitrine disponíveis para venda no varejo no local e online, armazenados no depósito da empresa.
* Sistemas de gestão, software e serviços para contabilidade, telecomunicações, banco de dados, segurança, comércio eletrônico e gestão de estoque.
* Acesso à Internet e a rede interna.
* Sistemas de retenção e armazenamento de dados.
* Sistemas legados em fim de vida útil que requerem monitoramento humano.

### Objetivos
O principal objetivo foi avaliar os ativos existentes e preencher a lista de verificação de controles e conformidade para determinar quais práticas precisam ser implementadas para melhorar a postura de segurança da Botium Toys.

---

## 3. Avaliação de Risco e Principais Descobertas

A avaliação inicial identificou uma **pontuação de risco de 8 em 10**, considerada alta. Esse risco elevado deve-se à falta de controles adequados e à não adesão às melhores práticas de conformidade.

### Descobertas Críticas:
* **Gestão de Acesso Inadequada**: Atualmente, todos os funcionários da Botium Toys têm acesso a dados armazenados internamente, incluindo dados de titulares de cartão e PII/SPII dos clientes. Controles de acesso baseados no princípio do privilégio mínimo e na separação de tarefas não foram implementados.
* **Falta de Criptografia**: A criptografia não é utilizada para garantir a confidencialidade das informações de cartão de crédito dos clientes que são aceitas, processadas, transmitidas e armazenadas internamente.
* **Ausência de Recuperação de Desastres**: A empresa não possui planos de recuperação de desastres atualmente em vigor. Adicionalmente, a empresa não possui backups de dados críticos.
* **Políticas de Senha Fracas**: Embora exista uma política de senha, seus requisitos são nominais e não estão alinhados com os requisitos mínimos atuais de complexidade. Não há um sistema de gerenciamento de senhas centralizado para impor tais requisitos.
* **Falta de Detecção de Intrusão**: O departamento de TI não instalou um sistema de detecção de intrusão (IDS).
* **Sistemas Legados**: Embora os sistemas legados sejam monitorados, não há um cronograma regular para essas tarefas e os métodos de intervenção não são claros.

### Pontos Fortes Identificados:
* **Segurança Física**: A localização física da loja possui fechaduras suficientes, vigilância por circuito fechado de televisão (CCTV) atualizada e sistemas de detecção e prevenção de incêndio em funcionamento.
* **Segurança de Perímetro**: Há um firewall implementado que bloqueia tráfego com base em um conjunto de regras de segurança definido adequadamente.
* **Proteção contra Malware**: O software antivírus está instalado e é monitorado regularmente pelo departamento de TI.
* **Conformidade Parcial com GDPR**: Já existe um plano para notificar os clientes da UE em até 72 horas em caso de violação de segurança. Políticas e procedimentos de privacidade foram desenvolvidos para documentar e manter os dados adequadamente.

---

## 4. Recomendações Prioritárias

Com base nas descobertas, as seguintes medidas foram recomendadas como urgentes para mitigar as brechas de segurança.

### Controles Preventivos
* **Implementar o Princípio do Menor Privilégio**: Garantir que os usuários tenham acesso apenas ao que é necessário para suas funções.
* **Fortalecer as Políticas de Senha**: Implementar políticas de senhas complexas para reduzir as chances de comprometimento de contas por ataques de força bruta ou de dicionário.
* **Monitoramento e Manutenção de Sistemas Legados**: Realizar monitoramento, manutenção e intervenção manual para identificar e gerenciar ameaças em sistemas desatualizados.

### Controles Corretivos
* **Desenvolver um Plano de Recuperação de Desastres**: Implementar um plano formal, pois a empresa não possui um atualmente.
* **Implementar uma Política de Backup**: Adotar uma política diária de backups.

---

## 5. Estrutura do Repositório

* **/relatorios**: Contém os documentos completos da auditoria.
    * `1_escopo_objetivos_e_avaliacao_de_risco.pdf`: Detalha o escopo, objetivos e a análise de risco inicial.
    * `2_lista_de_verificacao_controles_e_conformidade.docx`: Apresenta a checklist preenchida de controles e conformidade com PCI DSS, GDPR e SOC, incluindo as recomendações finais.
