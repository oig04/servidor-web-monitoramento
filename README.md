# Servidor Web com Monitoramento e Webhook

Este projeto é um servidor web básico configurado com **Nginx**, monitoramento de disponibilidade e integração com **webhooks** para alertas em tempo real, caso o servidor fique offline.

## O que já está pronto

- **Servidor Web**: O Nginx foi configurado com sucesso e está respondendo corretamente.
- **Monitoramento**: O script de monitoramento está configurado, mas ainda não foi completamente testado. O script verifica a disponibilidade do servidor a cada minuto e envia alertas caso o servidor fique offline.

## Como rodar o projeto

### 1. Clonar o repositório:
```bash
git clone https://github.com/oig04/servidor-web-monitoramento.git
cd servidor-web-monitoramento
=======
# Sistema de Monitoramento Ativo

## Descrição do Projeto

Este projeto faz parte do estágio de **DevSecOps** e tem como objetivo a criação de um sistema de monitoramento contínuo de servidores. A ideia é garantir a disponibilidade e estabilidade de um servidor web, com alertas automáticos via Telegram para notificar em tempo real sobre possíveis falhas ou quedas. O sistema foi configurado com **Nginx** e utiliza um script Bash para monitorar a conectividade do servidor, enviando alertas de maneira eficiente.

## Tecnologias Utilizadas

- **Nginx**: Servidor web responsável por hospedar a página de monitoramento.
- **Bash Script**: Implementação do script de monitoramento que verifica a disponibilidade do servidor a cada minuto.
- **Telegram API**: Comunicação com o Telegram para envio de alertas sobre o status do servidor.
- **Ubuntu (Linux)**: Sistema operacional utilizado durante o desenvolvimento e testes.
- **Git**: Controle de versão para o repositório de código-fonte.

## Funcionalidades

- **Monitoramento de Disponibilidade**: O script de monitoramento verifica a cada 1 minuto se o servidor está acessível via HTTP.
- **Alertas Automatizados**: Se o servidor estiver fora do ar, o sistema envia automaticamente uma notificação para o canal do Telegram.
- **Página HTML Personalizada**: A página de monitoramento exibe um design simples, mas eficaz, que informa o status do servidor.

## Objetivos do Projeto

- **Garantir Alta Disponibilidade**: A principal motivação deste projeto é garantir que o servidor esteja sempre disponível, evitando que falhas não sejam detectadas de maneira imediata.
- **Automatização de Processos**: Com a criação do script automatizado de monitoramento e notificação, reduz-se a necessidade de intervenção manual.
- **Aprimoramento Profissional**: Este projeto serviu como um excelente exercício para aprimorar meus conhecimentos de **DevSecOps**, **administração de servidores** e **integração de sistemas de notificação**.

## Como Rodar o Projeto

### Pré-requisitos

1. **Ubuntu 20.04 ou superior** (ou outra distribuição Linux similar).
2. **Nginx**: O servidor web para exibir a página.
3. **Telegram API**: Criação de um bot no Telegram para envio de mensagens.

### Passos de Instalação

1. **Instalar o Nginx**:
   ```bash
   sudo apt update
   sudo apt install nginx
   ```

2. **Clonar o repositório**:
   - Clone o repositório onde o código do projeto está hospedado.
   ```bash
   git clone <URL do seu repositório>
   ```

3. **Configuração do Nginx**:
   - Coloque o arquivo `index.html` personalizado em `/var/www/html/`:
   ```bash
   sudo cp index.html /var/www/html/
   ```

4. **Configuração do Script de Monitoramento**:
   - Abra e edite o script `monitorar_servidor.sh` para adicionar o `BOT_TOKEN` e `CHAT_ID` do seu bot do Telegram.
   ```bash
   nano monitorar_servidor.sh
   ```
   - Insira as informações do seu bot:
   ```bash
   BOT_TOKEN="seu_token_aqui"
   CHAT_ID="seu_chat_id_aqui"
   ```
- **Criando o Bot no Telegram**:
     1. Abra o Telegram e busque por **BotFather**.
     2. Envie o comando `/newbot` e siga as instruções para criar um novo bot.
     3. Após a criação, o BotFather fornecerá o `BOT_TOKEN`, que você precisará para autorizar seu bot a enviar mensagens.
     4. Para obter o `CHAT_ID` do Telegram, você pode iniciar uma conversa com o bot ou adicionar ele em um grupo e usar a API do Telegram para descobrir o ID ).
   - **Adicione o Token e o ID no Script**:
   ```bash
   BOT_TOKEN="seu_token_aqui"
   CHAT_ID="seu_chat_id_aqui"

5. **Rodar o Script de Monitoramento**:
   - Torne o script executável e rode-o:
   ```bash
   chmod +x monitorar_servidor.sh
   ./monitorar_servidor.sh
   ```

### Verificando a Página

Após configurar o Nginx e rodar o script de monitoramento, abra o navegador e acesse `http://localhost` ou o IP da máquina onde o servidor está rodando para verificar a página de monitoramento personalizada.

## Considerações Finais

Este projeto foi uma excelente oportunidade para aplicar meus conhecimentos de **infraestrutura como código**, **automação de monitoramento** e **comunicação com APIs externas**. Além disso, serviu para reforçar a importância de garantir a estabilidade de sistemas críticos em ambientes de produção.


## Links

- **GitHub**: [Giovanna Freitas](https://github.com/oig04)
