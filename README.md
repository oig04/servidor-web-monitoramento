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
