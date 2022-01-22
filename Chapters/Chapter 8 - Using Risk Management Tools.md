# Risk Types

1. Internal x External
2. IP(Intellectual Property) Theft
3. Software Compliance Licensing
4. Legacy Systems

# Risk Management

1. **Risk Awareness** : Basicamente estar ciente do risco
2. **Inherent Risk** : Que existe desde antes da construção do Software
3. **Residual Risk** : Risco restante após tentar mitigar ou gerenciar
4. **Control Risk** : Risco que existe por conta da necessidade de se ter mecanismos de controle para riscos
5. **Risk Appetite** : Quantidade de risco que a organização está disposta a aceitar

**Insurance** é transferir o risco para third-party entities

# Risk Assesment/Analysis
Em ordem:
1. Identificar os assets de valor
2. Ver as threats/vulns dos Assets
   
## Tipos de Análise

1. **Qualitativa** : falando de forma subjetiva sobre os riscos
2. **Quantitativa** : Fala do risco associando a um valor em dinheiro. Tendo como medidas SLE(Single Loss Expectancy), ARO(Annual Rate of Occurence) e ALE(Annual Loss Expectancy) sendo SLE x ARO

## Risk Register

Documento extenso acerca dos riscos

## Risk Matrix e Risk Heatmap

Representações visuais dos dados de riscos

# Network Scanners

**Scanless** é um Python based online tool para fazer port Scan

## Tipos

1. ARP ping e SYN Stealth Scan (Ambos para ver o host)
2. Port Scan (para ver a porta)
3. Service Scan (PPara ver o protocolo ou serviço)
4. OS Scan (Vê as diferenças nos pacotes TCP/IP para deduzir o OS)

## Detalhamento

| Credentialed Scan | Non-Credentialed Scan |
| ---------- | --------- |
| Usuário interno loga uma conta para o Scan ter mais privilégios e retornar mais detalhes | Sem nenhum tipo de privilégio |

# Frameworks de Segurança

| Framework | Utilidade |
| ---------- | --------- |
| PCI DSS | Framework de Segurança de transações de Cartão de Crédito |
| ISO 27001 | Framework de Segurança de Security Management |
| ISO 27701 | Framework de Segurança de Data Protection |

# Últimos conhecimentos

| Footprint | Fingerprinting |
| ---------- | --------- |
| Recoinessence/Escanear redes | Dados e metadados específicos de um APP ou OS |

**Pivoting** é usar um exploited system para atacar outros\

**Netflow** é um protocolo criado pela CISCO para exportar estatísticas de rede dos roteadores e switches em relação ao tráfego de dados\

**Rules of Engagement** : Define as regras num teste/implementação de segurança\

**Threat Hunting** : Actively Hunt threats before tools find them. Faz parte de Threat Hunting:
1. Intelligence Fusion(combina dados de threats)
2. Advisories and bulletins
3. Threat Feeds(describe threats)
4. Predictions of attackers behavior

**Outsorce** é terceirizar algo, como o desenvolvimento de um software.

## Ferramentas TCP

| TCPReplay | TCPDump |
| ---------- | --------- |
| Ferramenta para imitar e editar pacotes TCP. Muito útil para imitar ataques e testar se o IDS os detecta. | Protocol Analyser assim como o Wireshark |



