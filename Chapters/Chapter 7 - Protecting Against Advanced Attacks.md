# Attack Frameworks

## Cyber Kill Chain
1. Recon
2. Weaponization(Malware)
3. Delivery(Payload to target)
4. Exploitation
5. Installation
6. Command and Control
7. Actions and Objectives
   
## Diamond Model of Instrusion
(Do 1 ao 3 diz respeito ao atacante)
1. Adversary
2. Capabilities
3. Infrastructure
4. Victim

## Mitre ATT&CK(Adversarial Tactics, Techniques and Common Knowledge)
Uma matriz com 10 táticas e técnias para atingir cada um dos 10 ataques citados

# Ataques

## MITM
**Mais modernos MITM** criam duas conexões seguras com os dois alvos para decriptar as mensagens de um e encriptar novamente antes de mandar para o destino final. Pode revelear esse ataque:
1. **O delay** pode revelar o ataque
2. Os **certificados** não serem fornecidos por uma CA
3. **Fingerprint do SSH** muda caso um MITM seja criado depois de uma conexão já ter sido estabelecida

**SSL OU TLS Stripping** é um ataque que impede o SSL handshake da conexão HTTP, impedindo que se use o HTTPS após a conexão inicial do HTTP ser criada.\




## ARP
**ARP Poison** pode criar um MITM ou um DoS ao bagunçar a tabela ARP do roteador ou Switch\


| **ARP Request**  | **ARP Reply** |
| ---------- | --------- |
| Broadcast no IP desejado para saber qual é o MAC correspondente | Responde o ARP Request com o MAC certo quando o pacote é destinado ao dispositivo |

## MAC Flood

O Switch guarda a relação MAC x Interface de saída em uma tabela. Ao injetar muitos dados com MAC novos em uma determinada interface, essa tabela começa a aumentar até o ponto que dá um overflow e o Switch começa a se portar como um HUB. Alguns Switches se protegem com uma tabela ilimitada que, ao lotar, faz com que o Switch emita um SNMP trap para o administrador. 

## DNS Sinkhole

É um servidor que fornece resoluções Nome-IP errôneas. Pode ser usado por bem, para evitar que dispositivos infectados com malwares se conectem a domínios conhecidos por serem servidores de Command and Control; assim como também pode ser usado para o mal seja para DoS ou redirecionamento de páginas falsas.

## HTTP Headers

### HTTP Strict
Transport Security só mostra a página se for HTTPS
### Content-Security-Policy 
Define múltiplas fontes de conteúdo permitidas, como fontes permitidas de scripts, CSS, imagem

## Secure Cookie
Cookie com atributo de só ser transmitido através do protocolo HTTPS

# Análise de Software

| Static Analysis | Dynamic Analysis |
| ---------- | --------- |
| Scan de Código | Executa o código para ver os outputs |
| Manual code Review | Pode usar Fuzzy para enviar inputs aleatórios em busca de vulnerabilidades | 

# Ambientes de Desenvolvimento

1. Development
2. Test
3. Staging(Simula o ambiente de produção, usado para late-stage test)
4. Production
5. QA(Usado em cada estágio para garantir qualidade)

# Normalization
Basicamente reduzir redundância em um banco de dados
## First Normal Form(1NF)
1. Cada linha é única e tem Primary Key
2. Dados relacionados estão em outras tabelas
3. Nenhuma coluna possui grupos repetidos

## Second Normal Form(2NF)
1. Está na 1NF
2. Cada coluna depende da PK

## Third Normal Form(3NF)
2NF + algum nível de normalização


# Identificando Scripts nos Logs

Power shell usa "Invoke-Command" que podem estar nos logs, enquannto bash scripts podem ser detectados pois chamam /bin/bash e usam comandos "sh" ou "bash"

# Memory Leak
É um bug que faz uma aplicação consumir mais memórias do que deveria

# Injection Attacks
1. **Dynamic Link Library(DLL)** : Alocar uma DLL/lib maliciosa a um Software Integro para executar vírus
2. **LDAP** : Protocolo usado para se autenticar no AD, geralmente usa query num banco de dados para se autenticar, sendo assim é possível fazer um Injection Attack com o propósito de bypassar a autenticação
3. **XML Injection**
4. **Directory Traversal** : Ataque de injeção que visa acessar um arquivo colocando o full path dele
5. **XSS** : Persistente(Cujo código fica escrito) x Não Persistente
6. **Cross Site Request Forgery** : Modificar a URL para fazer uma URL maliciosa

## Proteção contra injection

**Stored Procedures** protegem contra SQL injection pois são procedimentos SQL prontos e testados


