# FNRC 2026.2 — Projeto Final (Grupo X)

Repositório do Projeto Final da disciplina **Fundamentos de Redes de Computadores**
do curso de **Bacharelado em Sistemas de Informação (BSI)** do
**Instituto Federal de Alagoas (IFAL) – Campus Maceió**, semestre letivo **2026.02**.

## Objetivo

Montar uma rede virtualizada com **8 VMs Ubuntu Server 22.04 LTS** distribuídas em
**4 PCs do laboratório**, todas com o adaptador de rede em modo **Placa em Ponte
(Bridge)**, aplicando na prática os conceitos de endereçamento, resolução de nomes,
acesso remoto e administração de usuários.

## Especificações

- **Sub-rede do grupo:** `192.168.26.(16 × X)/28`, em que X é o número do grupo
- **Endereçamento:** IP estático em todas as VMs (Netplan)
- **Nomes:** hostname e FQDN no domínio `grupoX.bsi-26-2.maceio.lab`
- **Resolução local:** arquivo `/etc/hosts` configurado em todas as máquinas
- **Usuários:** contas de todos os integrantes criadas em todas as VMs
- **Hipervisor:** VirtualBox (1 vCPU, 32 GB de disco, 512 MB de RAM após a instalação)

## Evidências de entrega

- Testes de conectividade com `ping` entre as VMs
- Acessos remotos com `ssh`
- Execução do script de validação da rede

## Estrutura do repositório

(Ajustar conforme a organização do grupo)

- `docs/` — documentação, tabela de endereçamento e diagrama da rede
- `scripts/` — script de validação e demais automações
- `evidencias/` — capturas de tela e saídas dos testes

## Integrantes

| Nome | Usuário |
|------|---------|
|      |         |

## Referências

- KUROSE, J. F.; ROSS, K. W. *Redes de Computadores e a Internet*. 8. ed. Pearson, 2022.
- LACROIX, J. *Mastering Ubuntu Server*. 4. ed. Packt, 2023.
- SOYINKA, W. *Linux Administration: A Beginner's Guide*. 8. ed. McGraw-Hill, 2020.
