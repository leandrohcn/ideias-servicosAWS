<div align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/93/Amazon_Web_Services_Logo.svg/2560px-Amazon_Web_Services_Logo.svg.png" width="200" alt="Logo AWS">
  <h1>Relatório de Implantação de Serviços AWS</h1>
  <h3>Projeto de Otimização de Custos para Farma-Certa</h3>
</div>

<br>

| **Empresa** | **Responsável pelo Projeto** | **Data de Início** |
| :--- | :--- | :--- |
| 💊 Farma-Certa | Leandro Neves | 29/08/2025 |

<br>

## 🎯 INTRODUÇÃO

> Este relatório apresenta o processo de implementação de ferramentas na empresa **Farma-Certa**. O objetivo do projeto foi elencar 3 serviços AWS com a finalidade de realizar **diminuição de custos imediatos**, otimizando a infraestrutura de TI existente e garantindo a sustentabilidade financeira da operação na nuvem.

---

## 🛠️ DESCRIÇÃO DO PROJETO

O projeto foi dividido em 3 etapas estratégicas para maximizar a economia de forma rápida e eficiente.

### Etapa 1: Controle e Visibilidade Financeira

- #### 💰 Nome da Ferramenta
  `AWS Budgets`

- #### 🎯 Foco da Ferramenta
  Controle proativo e alertas de custos.

- #### 📄 Descrição do Caso de Uso
  Para evitar gastos inesperados e garantir que a fatura da AWS se mantenha dentro do planejado, foi implementado o AWS Budgets. Configuramos um orçamento mensal de R$ 1.500,00 e criamos alertas automáticos que notificam os gestores via e-mail quando os custos atingem `50%`, `80%` e `95%` do valor orçado.
  
  **Resultado Imediato:** Ação proativa para corrigir anomalias de custo antes do fim do mês, **eliminando gastos excessivos e garantindo previsibilidade financeira.**

---

### Etapa 2: Otimização de Custos de Computação

- #### ⏱️ Nome da Ferramenta
  `AWS Instance Scheduler`

- #### 🎯 Foco da Ferramenta
  Automatização para ligar/desligar instâncias EC2.

- #### 📄 Descrição do Caso de Uso
  A Farma-Certa utiliza um servidor (instância EC2) para seu sistema de gestão de estoque e um ambiente de testes. Foi identificado que esses servidores só precisam operar durante o horário comercial (Segunda a Sábado, das 8h às 20h). Com o AWS Instance Scheduler, foi criada uma agenda para desligar automaticamente essas instâncias fora do expediente e nos domingos.

  **Resultado Imediato:** **Redução de aproximadamente 55% na fatura dessas instâncias**, pois a cobrança cessa completamente quando elas não estão em uso.

---

### Etapa 3: Redução de Custos de Armazenamento

- #### 🗄️ Nome da Ferramenta
  `Amazon S3 Intelligent-Tiering`

- #### 🎯 Foco da Ferramenta
  Automatização da otimização de custos de armazenamento.

- #### 📄 Descrição do Caso de Uso
  A farmácia armazena um grande volume de dados de longo prazo, como receitas digitalizadas e notas fiscais. Esses arquivos são acessados com frequência no primeiro mês, mas raramente depois disso. Utilizando a classe S3 Intelligent-Tiering, os objetos são movidos automaticamente para camadas de armazenamento mais baratas (Acesso Infrequente e Arquivo) quando deixam de ser acessados.

  **Resultado Imediato:** **Redução contínua no custo mensal de armazenamento de até 70%** para dados antigos, sem a necessidade de gerenciamento manual.
