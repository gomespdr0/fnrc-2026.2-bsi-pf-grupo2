# Endereçamento e Nomes — Grupo 2

Documento de endereçamento da rede virtualizada do **Grupo 2**
(FNRC 2026.2 — BSI/IFAL Campus Maceió).

## Integrantes

| Aluno | Nome | Usuário da VM |
|-------|------|---------------|
| Aluno 1 | Caio Vinícius | |
| Aluno 2 | Marcos Antonio | |
| Aluno 3 | Pedro Gomes | |
| Aluno 4 | Wagner Leandro | |

## Sub-rede

A sub-rede do grupo segue a regra `192.168.26.(16 × X)/28`, com X = 2.

| Item | Valor |
|------|-------|
| Endereço da sub-rede | `192.168.26.32` |
| Máscara | `255.255.255.240` (`/28`) |
| Endereço de broadcast | `192.168.26.47` |
| Faixa de hosts utilizáveis | `192.168.26.33` a `192.168.26.46` (14 endereços) |
| Domínio (zona) | `grupo2.bsi-26-2.maceio.lab` |

## Interfaces de rede

| Interface | Função | Situação |
|-----------|--------|----------|
| `enp0s3` | WAN | usada em todas as VMs |
| `enp0s8` | LAN | não usada |

## Tabela de VMs

| VM | Máquina física | Hostname | FQDN | Interface | IP/máscara |
|----|----------------|----------|------|-----------|------------|
| GW | PC1 | `g2-pc1-gw` | `g2-pc1-gw.grupo2.bsi-26-2.maceio.lab` | `enp0s3` | a definir |
| VM1 | PC1 | `g2-pc1-vm1` | `g2-pc1-vm1.grupo2.bsi-26-2.maceio.lab` | `enp0s3` | 192.168.26.__/28 |
| VM2 | PC1 | `g2-pc1-vm2` | `g2-pc1-vm2.grupo2.bsi-26-2.maceio.lab` | `enp0s3` | 192.168.26.__/28 |
| VM3 | PC2 | `g2-pc2-vm1` | `g2-pc2-vm1.grupo2.bsi-26-2.maceio.lab` | `enp0s3` | 192.168.26.__/28 |
| VM4 | PC2 | `g2-pc2-vm2` | `g2-pc2-vm2.grupo2.bsi-26-2.maceio.lab` | `enp0s3` | 192.168.26.__/28 |
| VM5 | PC3 | `g2-pc3-vm1` | `g2-pc3-vm1.grupo2.bsi-26-2.maceio.lab` | `enp0s3` | 192.168.26.__/28 |
| VM6 | PC3 | `g2-pc3-vm2` | `g2-pc3-vm2.grupo2.bsi-26-2.maceio.lab` | `enp0s3` | 192.168.26.__/28 |
| VM7 | PC4 | `g2-pc4-vm1` | `g2-pc4-vm1.grupo2.bsi-26-2.maceio.lab` | `enp0s3` | 192.168.26.__/28 |
| VM8 | PC4 | `g2-pc4-vm2` | `g2-pc4-vm2.grupo2.bsi-26-2.maceio.lab` | `enp0s3` | 192.168.26.__/28 |

## Convenção de nomes

Os hostnames seguem o padrão `g<grupo>-pc<número do PC>-vm<número da VM no PC>`
e o FQDN é `<hostname>.<grupo>.<turma>.maceio.lab`.

## Repositório

Link do projeto no GitHub: <https://github.com/USUARIO/fnrc-2026.2-bsi-pf-grupo2>
