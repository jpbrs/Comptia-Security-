# Segurança Física 

**Mobile Robots** são usados para monitorar datacenters contra intrusos\
**Two Person Integrity** se refere a precisar de duas pessoas autorizadas para executar determinada tarefa importante\
**CCTV** transmite dados de monitoramento de vídeo para monitores\
**Bollards** são barricadas efetivas e específicas para bloquear veículos. São aqueles cilindros de metal na vertical\
**Vendor Diversity** é a técnica de usar uma diversidade de soluções de segurança de diversos vendedores para garantir segurança em multiplos níveis\
**Technology Diversity** é usar uma variedade de tecnologias com o propósito de fornecer mais segurança\
**Air Gap** é separar/isolar fisicamente um computador ou rede\
**Vaults** é um quarto ou compartimento usado para guardar itens de valor\
**Safes** são tipo lockers ou cofres\
**Hot and Cold Aisles** são corredores de ar quente ou frio que regulam as tempraturas do datacenter\
**Access Control Vestibules ou Mantraps** são espécies de passagens que permitem apenas 1 funcionários passar por vez. São 2 portas, sendo que a segunda só abre quando a primeira fechar\

# Redundâncias
Redundâncias servem para evitar que se criem Single Points of Failure

**Multipath** é uma técnica de tolerância à falhas que provê mais de um caminho para um sistema de armazenamento

## Redundâncias de Disco

**RAID(Redundant Array of independent disks)** é a tecnologia usada para adicionar redundâncias aos discos para caso algum deles falhe

| Tecnologia | Descrição |
| ---------- | --------- |
| RAID 0 | Não provê redundância ou tolerância a falha, apenas aumenta a performance de Leitura e Escrita ao separar os dois ou mais discoc |
| RAID 1 | Espelha um disco em outro disco para garantir redundância. Nesse caso, o RAID 1 sobrevive a perda de 1 disco |
| RAID 5 ou 6 | RAID 5 é 3 ou mais discos e RAID 6 são 4 ou mais, assim o RAID 5 sobrevive a perda de 1 disco e 6 a perda de 2 |
| RAID 10 | É o RAID 1 + 0, une a capacidade dos dois RAIDs, com no mínimo 4 discos |

## Redundância no Servidor

Pode ser criado adicionando servidores e aplicando Load Balancing

### Tipos de Load Balancing

1. **Ativo/Ativo** : Todos os servers online e o tráfego é balanceado
2. **Ativo/Passivo** : Um server online e outro offline, apenas liga em caso de falha

## Redundância de NIC

NIC teaming é fazer um aglomerado de NICs para suportar o tráfego em conjunto, caso uma falhe, ainda existem outras

## Redundância de Energia

UPS(Uninterruptable Power Supply), dupla alimentação, geradores, etc.

# Backups

Pode ser feitos em fitas, discos, nuvem ou em qualquer formato. **É mais comum se fazer em fitas por conta da capacidade de armazenamento, preço e por ser física**

| Backup Online(Hot) | Backup Offline(Cold) |
| ---------- | --------- |
| Na cloud | Local |
| Faz Backup enquanto o DB está operando | Feito quando o banco de dados não está operando |

## Tipos de Backups

1. **Full** : Todos os dados
2. **Differential** : Apenas dados alterados desde o último Full Backup
3. **Incremental** : Dados diferentes desde o último Full Backup ou Backup Incremental
4. **Snapshot/Image** : Geralmente feito em VMs, são backups dos dados em um determinado momento do tempo

# Planos de Recuperação à Falhas

**Business Continuity Plan** é um plano que inclui recuperação de desastres, planos para voltar a operação após uma crise\
**Business Impact Analysis** avalia os cenários e prejuízos envolvendo desastres. Identifica os componentes críticos para o funcionamento ou sucesso de uma organização \
**Continuity of Operations Planning** foca em reestabelecer as operações essenciais para o funcionamento do sistema\


| Recovery Time Objective (RTO) | Recovery Point Objective (RPO) |
| ---------- | --------- |
| Explicita o tempo máximo que o sistema suporta uma crise | Explicita a maxima quantidade de dados ou recursos que podem ser perdidos e mesmo assim manter o sistema funcionando |

## Treinamentos para treinar funcionários em casos de crises

1. Simulações
2. Tabletop : Conversa sobre o que fazer em situações de emergência, com objetivo de fazer com que os funcionários participem verbalmente


| Cold Site | Hot Site |
| ---------- | --------- |
| Site com energia para funcionar, mas com um plano de recuperação sem urgências | Dados atualizados, funciona 24/7 e se recupera rápido de desastres |

Obviamente o custo do Hot Site é muito superior ao do Cold

# Outros

**Credit Card Skimmer** é capturar dados de cartão de crédito em pontos de vendas\
