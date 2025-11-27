<div align="center">
  <h1>🏛️ AUREUS</h1>
  <h3>High-Throughput Financial Ledger Engine</h3>
  <p>
    Um motor de transações financeiras distribuído, focado em consistência ACID, concorrência extrema e idempotência.
  </p>
  
  ![Go](https://img.shields.io/badge/Go-1.21+-00ADD8?style=for-the-badge&logo=go)
  ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-16-316192?style=for-the-badge&logo=postgresql)
  ![Docker](https://img.shields.io/badge/Docker-Enabled-2496ED?style=for-the-badge&logo=docker)
  ![Architecture](https://img.shields.io/badge/Architecture-Hexagonal-orange?style=for-the-badge)

</div>

---

## 📖 Sobre o Projeto

**Aureus** (do latim, moeda de ouro) é um Core Banking Ledger simplificado, projetado para resolver os problemas mais críticos de sistemas financeiros modernos: **Race Conditions**, **Deadlocks** e **Double-Spending**.

Diferente de APIs REST comuns, o Aureus foi arquitetado para suportar alta carga de transações simultâneas (ex: processamento de PIX em massa ou Settlements de cartão), garantindo que o saldo nunca fique negativo e que cada centavo seja auditável.

> ⚠️ **Nota:** Este repositório contém a **documentação técnica e arquitetural** do projeto. O código-fonte do motor é proprietário. Para discussões sobre a implementação ou acesso ao código para fins de recrutamento/auditoria, entre em contato comigo.

---

## 🏗️ Arquitetura

O sistema segue os princípios de microserviços e arquitetura hexagonal, garantindo alta coesão e baixo acoplamento entre os componentes. A comunicação entre serviços é realizada via RabbitMQ para máxima performance.

## Microserviços Principais

- **Transaction Processor:** Responsável por validar e processar transações financeiras. ⏳
- **Account Manager:** Gerencia contas de usuários e seus saldos. ⏳
- **Audit Logger:** Mantém um log imutável de todas as transações para auditoria.⏳
- **Notification Service:** Envia notificações sobre transações e alertas de saldo.⏳
- **API Gateway:** Ponto de entrada unificado para todas as requisições externas.⏳
- **Database Service:** Interface com o banco de dados PostgreSQL, garantindo operações ACID.⏳
- **Load Balancer:** Distribui a carga de requisições entre múltiplas instâncias dos serviços.⏳
- **Cache Layer:** Utiliza Redis para acelerar consultas frequentes e reduzir a latência.⏳
- **Monitoring Service:** Coleta métricas e logs para monitoramento em tempo real.⏳
- **Authentication Service:** Gerencia autenticação e autorização de usuários.⏳
- **Backup Service:** Realiza backups periódicos do banco de dados para garantir a recuperação de dados.⏳
- **Configuration Service:** Centraliza a gestão de configurações dos microserviços.⏳
- **Rate Limiter:** Controla o fluxo de requisições para evitar sobrecarga do sistema.⏳
- **Scheduler Service:** Gerencia tarefas agendadas, como liquidações periódicas.⏳
- **Reporting Service:** Gera relatórios financeiros e estatísticas de uso.⏳
- **Fraud Detection Service:** Monitora transações suspeitas e previne fraudes.⏳
- **Settlement Service:** Gerencia o processo de liquidação entre diferentes instituições financeiras.⏳

## Tecnologias Utilizadas

- **Linguagem de Programação:** Go (Golang)
- **Banco de Dados:** PostgreSQL
- **Containerização:** Docker
- **Comunicação entre Serviços:** RabbitMQ
- **Cache:** Redis
- **Monitoramento:** Prometheus e Grafana
- **Autenticação:** JWT (JSON Web Tokens)
- **Controle de Versão:** Git
- **Plataforma de Hospedagem:** Self-hosted (Home Lab)
- **CI/CD:** GitHub Actions

## 🚀 Como Contribuir

Contribuições são bem-vindas! Se você deseja ajudar a melhorar o Aureus, entre em contato comigo para discutir possíveis colaborações.

## 📄 Licença

Esse projeto é proprietário. Para mais informações sobre licenciamento, entre em contato comigo diretamente.

## 📞 Contato

- Nome: Vitor Amaral de Melo
- Email: vitor.amaral10@gmail.com
- LinkedIn: [linkedin.com/in/vitoramaral10](https://www.linkedin.com/in/vitoramaral10/)
- GitHub: [github.com/vitoramaral10](https://github.com/vitoramaral10)
- Portfólio: [vitoramaral.dev](https://vitoramaral.dev)
- X: [@beybnoky](https://x.com/beybnoky)
