# Desafio de Projeto: Implementando Monitoramento no Azure

Repositório criado para o Desafio de Projeto da DIO sobre a implementação de monitoramento de recursos na nuvem Microsoft Azure.

## 📖 Descrição

O objetivo deste projeto foi configurar um sistema de monitoramento para uma Máquina Virtual (VM) no Azure, com o intuito de gerar um alerta específico quando a VM fosse excluída. O processo foi documentado para servir como um guia prático e material de estudo.

## 🛠️ Ferramentas Utilizadas
* Microsoft Azure
* Azure Monitor
* Máquinas Virtuais (VMs)
* Grupos de Ações (Action Groups)
* Regras de Alerta (Alert Rules)
* GitHub

## ⚙️ Implementação

### 1. Criação dos Recursos no Azure
Inicialmente, foi criado um Grupo de Recursos para organizar os serviços. Em seguida, uma Máquina Virtual (`vm-monitorada`) foi provisionada para ser o alvo do monitoramento.

### 2. Configuração da Regra de Alerta
Utilizando o Azure Monitor, foi criada uma Regra de Alerta com as seguintes especificações:
* **Escopo:** A Máquina Virtual `vm-monitorada`.
* **Condição:** O sinal de Log de Atividades "Excluir Máquina Virtual (Virtual Machines)".
* **Ação:** Foi configurado um Grupo de Ações para notificar um e-mail pré-definido sempre que o alerta fosse
