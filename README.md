# FNRC 2026.2 — Projeto Final (Grupo 2)

Repositório do Projeto Final da disciplina **Fundamentos de Redes de Computadores**
do curso de **Bacharelado em Sistemas de Informação (BSI)** do
**Instituto Federal de Alagoas (IFAL) – Campus Maceió**, semestre letivo **2026.02**.

## Objetivo

Montar uma rede virtualizada com **8 VMs Ubuntu Server 22.04 LTS** distribuídas em
**4 PCs do laboratório**, todas com o adaptador de rede em modo **Placa em Ponte
(Bridge)**, aplicando na prática endereçamento IP, resolução de nomes, acesso
remoto e administração de usuários.

## Integrantes

| Aluno | Nome | Usuário da VM |
|-------|------|---------------|
| Aluno 1 | Caio Vinícius | |
| Aluno 2 | Marcos Antonio | |
| Aluno 3 | Pedro Gomes | |
| Aluno 4 | Wagner Leandro | |

## Rede do Grupo 2

| Item | Valor |
|------|-------|
| Sub-rede | `192.168.26.32/28` |
| Máscara | `255.255.255.240` |
| Broadcast | `192.168.26.47` |
| Hosts utilizáveis | `192.168.26.33` a `192.168.26.46` |
| Domínio (zona) | `grupo2.bsi-26-2.maceio.lab` |
| Interface em uso (WAN) | `enp0s3` |
| Interface LAN (`enp0s8`) | não usada |
| Endereçamento | IP estático (Netplan) em todas as VMs |

## Máquinas e nomes (FQDN)

| PC | VM | Hostname | FQDN |
|----|----|----------|------|
| PC1 | GW | `g2-pc1-gw` | `g2-pc1-gw.grupo2.bsi-26-2.maceio.lab` |
| PC1 | VM1 | `g2-pc1-vm1` | `g2-pc1-vm1.grupo2.bsi-26-2.maceio.lab` |
| PC1 | VM2 | `g2-pc1-vm2` | `g2-pc1-vm2.grupo2.bsi-26-2.maceio.lab` |
| PC2 | VM3 | `g2-pc2-vm1` | `g2-pc2-vm1.grupo2.bsi-26-2.maceio.lab` |
| PC2 | VM4 | `g2-pc2-vm2` | `g2-pc2-vm2.grupo2.bsi-26-2.maceio.lab` |
| PC3 | VM5 | `g2-pc3-vm1` | `g2-pc3-vm1.grupo2.bsi-26-2.maceio.lab` |
| PC3 | VM6 | `g2-pc3-vm2` | `g2-pc3-vm2.grupo2.bsi-26-2.maceio.lab` |
| PC4 | VM7 | `g2-pc4-vm1` | `g2-pc4-vm1.grupo2.bsi-26-2.maceio.lab` |
| PC4 | VM8 | `g2-pc4-vm2` | `g2-pc4-vm2.grupo2.bsi-26-2.maceio.lab` |

O detalhamento dos IPs de cada VM está em [`docs/enderecamento.md`](docs/enderecamento.md).

## Requisitos atendidos

- IP estático em todas as VMs
- Hostname e FQDN no domínio `grupo2.bsi-26-2.maceio.lab`
- Arquivo `/etc/hosts` configurado em todas as máquinas
- Usuários de todos os integrantes criados em todas as VMs
- Testes de `ping` e `ssh` entre as VMs
- Script de validação da rede

## Estrutura do repositório

- `docs/` — endereçamento, topologia, procedimentos e problemas encontrados
- `configs/` — arquivos Netplan e `/etc/hosts` de cada VM
- `scripts/` — criação de usuários e validação da rede
- `evidencias/` — saídas e capturas dos testes de `ping`, `ssh` e validação

## Referências

- KUROSE, J. F.; ROSS, K. W. *Redes de Computadores e a Internet*. 8. ed. Pearson, 2022.
- LACROIX, J. *Mastering Ubuntu Server*. 4. ed. Packt, 2023.
- SOYINKA, W. *Linux Administration: A Beginner's Guide*. 8. ed. McGraw-Hill, 2020.
