# Configuração e Validação do Firewall

## Objetivo

Configurar o UFW (Uncomplicated Firewall) para proteger o servidor e validar que os serviços continuam acessíveis.

## Requisitos

- SSH permitido para administração remota.
- HTTP permitido para acesso web.
- HTTPS permitido apenas quando configurado.
- Firewall ativo.
- Regras validadas.
- Serviço web validado após ativação do firewall.

## Ficheiros

- firewall.md
- validacao.md

## Comandos principais

Verificar estado:

```bash
sudo ufw status verbose
