# Walletly

**Walletly** é uma plataforma de **gestão financeira pessoal** focada em transformar dados financeiros brutos em **organização, previsibilidade e insights acionáveis**, enquanto evolui uma **arquitetura moderna e escalável**.

---

## Visão do Projeto

> Mais do que um produto, a Walletly é um **laboratório de arquitetura de software**.
> 
> O projeto foi idealizado e desenvolvido por [Pedro Figueiredo](https://www.github.com/Myourkiu).
> 
> Mantido de forma privada sob a organização [WalletlyLabs](https://www.github.com/WalletlyLabs).

Toda a concepção do sistema — **arquitetura, domínio, decisões técnicas e evolução estrutural** — é responsabilidade do autor.

Desde sua origem, a Walletly vai além da construção de um produto funcional. O projeto nasce com o propósito de evoluir continuamente sua arquitetura de software, explorando boas práticas de design de domínio, sistemas distribuídos, processamento assíncrono e integração de IA, sempre priorizando escalabilidade, manutenibilidade e clareza estrutural.

Posteriormente, o projeto também será utilizado como um ambiente prático de aprendizado em infraestrutura, aprofundando conhecimentos em Linux, SSH, firewall, proxy reverso, DNS, TLS, containerização, CI/CD, observabilidade e monitoramento, com o objetivo de dominar a base operacional de um sistema em produção para que uma futura migração para qualquer web service represente apenas uma camada de abstração.

---

## Objetivos Principais

* Importar dados financeiros via **CSV**
* Organizar transações de forma **automática e manual**
* Calcular **Previsibilidade Financeira**
* Gerar **insights financeiros com IA**
* Exibir dados de forma clara em **dashboards**
* Evoluir continuamente a **arquitetura do sistema**

---

## Como Funciona

### Fluxo Principal

1. Usuário cria uma conta
2. Usuário importa um arquivo **CSV**
3. O sistema inicia um fluxo assíncrono:
   * Evento publicado no **RabbitMQ**
   * Microsserviço consome o evento
   * CSV é processado e validado
   * Transações são categorizadas com **IA**
   * Dados persistidos no **PostgreSQL**
4. Backend atualiza o status do processamento
5. Dashboard consome dados agregados via **Redis**
6. Insights por IA são gerados de forma **assíncrona**

---

## Pilares Técnicos

* Arquitetura orientada a eventos
* Processamento assíncrono
* Microsserviços
* Cache para leitura otimizada
* IA desacoplada do fluxo principal
* Evolução contínua de domínio e arquitetura
* Boas práticas de código
* Escalabilidade (tanto API quanto banco de dados)
* DevOps/Infra

---

