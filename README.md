# Auditoria de Segurança e Conformidade: Estudo de Caso da Botium Toys

## 1. Resumo do Projeto

Este repositório contém os artefatos e a análise de uma auditoria de segurança da informação realizada na empresa fictícia Botium Toys. [cite_start]O objetivo foi avaliar a postura de segurança da empresa, identificar vulnerabilidades, verificar a conformidade com padrões relevantes e fornecer recomendações para mitigar os riscos encontrados[cite: 25].

---

## 2. Contexto e Objetivos

### Escopo
[cite_start]A auditoria abrangeu todo o programa de segurança da Botium Toys, incluindo todos os ativos gerenciados pelo departamento de TI, processos internos e procedimentos relacionados a controles de segurança e conformidade[cite: 23, 24]. Os ativos incluem:
* [cite_start]Equipamentos locais e de funcionários (desktops, laptops, smartphones)[cite: 28, 29].
* [cite_start]Produtos de vitrine armazenados no depósito[cite: 30].
* [cite_start]Sistemas de gestão (contabilidade, banco de dados, e-commerce, etc.)[cite: 31].
* [cite_start]Rede interna e acesso à Internet[cite: 32].
* [cite_start]Sistemas legados que exigem manutenção e monitoramento humano[cite: 34].

### Objetivos
[cite_start]O principal objetivo foi preencher as listas de verificação de controles e conformidade para identificar as lacunas existentes e determinar as ações necessárias para fortalecer a segurança da Botium Toys[cite: 25].

---

## 3. Avaliação de Risco e Principais Descobertas

[cite_start]A avaliação inicial identificou uma **pontuação de risco de 8 em 10**, considerada alta[cite: 43]. [cite_start]Esse risco elevado deve-se principalmente à falta de controles de segurança essenciais e à não adesão a melhores práticas de conformidade[cite: 44, 47].

### Descobertas Críticas:
* [cite_start]**Gestão de Acesso Inadequada**: Todos os funcionários possuem acesso a dados sensíveis, como informações de titulares de cartão (PCI) e dados de identificação pessoal (PII/SPII), pois não há controles de privilégio mínimo ou separação de funções implementados[cite: 49, 52].
* [cite_start]**Falta de Criptografia**: As informações de cartão de crédito dos clientes não são criptografadas, o que representa uma falha grave de conformidade com o PCI DSS[cite: 50].
* [cite_start]**Ausência de Recuperação de Desastres**: A empresa não possui um plano de recuperação de desastres e não realiza backups de dados críticos, colocando a continuidade dos negócios em risco[cite: 19, 20, 57].
* [cite_start]**Políticas de Senha Fracas**: A política de senhas existente é nominal e não segue os padrões mínimos de complexidade, além de não haver um sistema de gerenciamento centralizado[cite: 60, 61].
* [cite_start]**Falta de Detecção de Intrusão**: Não há um Sistema de Detecção de Intrusão (IDS) instalado para monitorar a rede em busca de atividades maliciosas[cite: 56].
* [cite_start]**Sistemas Legados**: O monitoramento e a manutenção de sistemas legados são realizados sem um cronograma regular ou métodos de intervenção claros[cite: 62].

### Pontos Fortes Identificados:
* [cite_start]**Segurança Física**: A empresa possui controles físicos adequados, como fechaduras, vigilância por CFTV e sistemas de detecção de incêndio[cite: 63].
* [cite_start]**Segurança de Perímetro**: Existe um firewall funcional que bloqueia tráfego com base em regras de segurança definidas[cite: 54].
* [cite_start]**Proteção contra Malware**: Software antivírus está instalado e é monitorado regularmente[cite: 55].
* [cite_start]**Conformidade Parcial com GDPR**: Já existe um plano para notificar clientes da UE em caso de violação de dados [cite: 58][cite_start], e políticas de privacidade foram desenvolvidas[cite: 59].

---

## 4. Recomendações Prioritárias

[cite_start]Com base nas descobertas, as seguintes medidas foram recomendadas como urgentes para mitigar as brechas de segurança identificadas[cite: 13].

### Controles Preventivos
* [cite_start]**Implementar o Princípio do Menor Privilégio**: Garantir que os usuários acessem apenas as informações estritamente necessárias para suas funções[cite: 15].
* [cite_start]**Fortalecer as Políticas de Senha**: Adotar requisitos de senhas complexas para reduzir o risco de ataques de força bruta ou de dicionário[cite: 16].
* [cite_start]**Monitoramento de Sistemas Legados**: Estabelecer um cronograma e procedimentos claros para o monitoramento, manutenção e intervenção em sistemas desatualizados[cite: 17].

### Controles Corretivos
* [cite_start]**Desenvolver um Plano de Recuperação de Desastres**: Criar e implementar um plano formal para garantir a continuidade dos negócios em caso de um incidente grave[cite: 19].
* [cite_start]**Implementar uma Política de Backup**: Realizar backups diários de todos os dados críticos da empresa[cite: 20].

---

## 5. Estrutura do Repositório

* **/relatorios**: Contém os documentos completos da auditoria.
    * [cite_start]`1_escopo_objetivos_e_avaliacao_de_risco.pdf`: Detalha o escopo, objetivos e a análise de risco inicial[cite: 21].
    * [cite_start]`2_lista_de_verificacao_controles_e_conformidade.docx`: Apresenta a checklist preenchida de controles e conformidade com PCI DSS, GDPR e SOC[cite: 1].
