# Auditoria de Segurança e Conformidade: Estudo de Caso da Botium Toys

## 1. Resumo do Projeto

Este repositório contém os artefatos e a análise de uma auditoria de segurança da informação realizada na empresa fictícia Botium Toys. O objetivo foi avaliar a postura de segurança da empresa, identificar vulnerabilidades, verificar a conformidade com padrões relevantes e fornecer recomendações para mitigar os riscos encontrados.

---

## 2. Contexto e Objetivos

### Escopo
[cite_start]O escopo da auditoria foi definido como todo o programa de segurança da Botium Toys[cite: 66]. [cite_start]Isso significa que todos os ativos, processos e procedimentos internos relacionados à implementação de controles e conformidade foram avaliados[cite: 67]. Os ativos incluem:
* [cite_start]Equipamento local para necessidades de negócios no escritório[cite: 71].
* [cite_start]Equipamentos de funcionários, como dispositivos de usuário final (desktops/laptops, smartphones), estações de trabalho remotas, fones de ouvido, entre outros[cite: 72].
* [cite_start]Produtos de vitrine disponíveis para venda, armazenados no depósito[cite: 73].
* [cite_start]Sistemas de gestão, software e serviços para contabilidade, telecomunicações, banco de dados, segurança, comércio eletrônico e gestão de estoque[cite: 74].
* [cite_start]Acesso à Internet [cite: 74] [cite_start]e a rede interna[cite: 75].
* [cite_start]Sistemas de retenção e armazenamento de dados[cite: 76].
* [cite_start]Sistemas legados em fim de vida útil que requerem monitoramento humano[cite: 77].

### Objetivos
[cite_start]O principal objetivo foi avaliar os ativos existentes e preencher a lista de verificação de controles e conformidade para determinar as ações necessárias para fortalecer a segurança da Botium Toys[cite: 68].

---

## 3. Avaliação de Risco e Principais Descobertas

[cite_start]A avaliação inicial identificou uma **pontuação de risco de 8 em 10**, considerada alta[cite: 86]. [cite_start]Esse risco elevado deve-se à falta de controles adequados e à não adesão às melhores práticas de conformidade[cite: 87].

### Descobertas Críticas:
* [cite_start]**Gestão de Acesso Inadequada**: Atualmente, todos os funcionários da Botium Toys têm acesso a dados armazenados internamente, incluindo dados de titulares de cartão e PII/SPII dos clientes[cite: 92]. [cite_start]Controles de acesso baseados no princípio do privilégio mínimo e na separação de tarefas não foram implementados[cite: 95].
* [cite_start]**Falta de Criptografia**: A criptografia não é utilizada para proteger as informações de cartão de crédito dos clientes que são aceitas, processadas, transmitidas e armazenadas internamente[cite: 93].
* [cite_start]**Ausência de Recuperação de Desastres**: A empresa não possui planos de recuperação de desastres[cite: 100]. [cite_start]Adicionalmente, não são feitos backups de dados críticos[cite: 100].
* [cite_start]**Políticas de Senha Fracas**: Embora exista uma política de senha, seus requisitos são nominais e não estão alinhados com os padrões atuais de complexidade[cite: 103]. [cite_start]Não há um sistema de gerenciamento de senhas centralizado para impor tais requisitos[cite: 104].
* [cite_start]**Falta de Detecção de Intrusão**: A empresa não instalou um sistema de detecção de intrusão (IDS)[cite: 99].
* [cite_start]**Sistemas Legados**: O monitoramento e a manutenção de sistemas legados são realizados sem um cronograma regular e os métodos de intervenção não são claros[cite: 105].

### Pontos Fortes Identificados:
* [cite_start]**Segurança Física**: A localização física da loja possui fechaduras adequadas, vigilância por CFTV atualizada e sistemas de detecção e prevenção de incêndio operacionais[cite: 106].
* [cite_start]**Segurança de Perímetro**: Há um firewall implementado que bloqueia tráfego com base em um conjunto de regras de segurança definido[cite: 97].
* [cite_start]**Proteção contra Malware**: O software antivírus está instalado e é monitorado regularmente pelo departamento de TI[cite: 98].
* [cite_start]**Conformidade Parcial com GDPR**: Já existe um plano para notificar os clientes da UE em até 72 horas em caso de violação de segurança[cite: 101]. [cite_start]Políticas e procedimentos de privacidade foram desenvolvidos para documentar e manter os dados adequadamente[cite: 102].

---

## 4. Recomendações Prioritárias

Com base nas descobertas, as seguintes medidas foram recomendadas como urgentes para mitigar as brechas de segurança.

### Controles Preventivos
* [cite_start]**Implementar o Princípio do Menor Privilégio**: Garantir que os usuários tenham acesso apenas ao que é necessário para suas funções[cite: 121].
* [cite_start]**Fortalecer as Políticas de Senha**: Implementar políticas de senhas complexas para reduzir as chances de comprometimento de contas[cite: 122].
* [cite_start]**Monitoramento e Manutenção de Sistemas Legados**: Realizar monitoramento, manutenção e intervenção manual para gerenciar ameaças em sistemas desatualizados[cite: 123].

### Controles Corretivos
* [cite_start]**Desenvolver um Plano de Recuperação de Desastres**: Implementar um plano formal, pois a empresa não possui um atualmente[cite: 125].
* [cite_start]**Implementar uma Política de Backup**: Realizar uma política diária de backups[cite: 126].

---

## 5. Estrutura do Repositório

* **/relatorios**: Contém os documentos completos da auditoria.
    * `1_escopo_objetivos_e_avaliacao_de_risco.pdf`: Detalha o escopo, objetivos e a análise de risco inicial.
    * `2_lista_de_verificacao_controles_e_conformidade.docx`: Apresenta a checklist preenchida de controles e conformidade com PCI DSS, GDPR e SOC, incluindo as recomendações finais.
