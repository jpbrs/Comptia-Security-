**ICMP, assim como PING, usa UDP na camada de transporte**

# Voice and Video
1. **RTP** usa VoIP para transmitir dados
2. **SRTP** é o RTP c/ crypto e integridade e autenticação. Usado para Unicast ou multicast
3. **SIP(Session Initiation Protocol)** serve para iniciar, manter e terminar as sessões de áudio e vídeio que usarão RTP ou SRTP. Ele não transporta dados, mas tem metadados que podem ser usados para ver quem ligou p/ quem

# File Transfer
1. **FTP** transporta arquivos em plain text
2. **TFTP** é Trivial FTP, usado para arquivos menores

# Criptografando dados
1. **SSH** criptografa dados de sessão ou arquivos como o SCP
2. **SSL** foi substituído, era usado para HTTPs e SNMP
3. **TLS** é o Upgrade do SSL
4. **Ipsec** é nativo do IPv6, mas disponível no IPv4, encripta os dados da camada de rede. **Usado para tunelamento em VPN**
5. **SFTP** é extensão so SSH, também usa porta 22
6. **FTPS** é FTP + TLS, portas 989 e 990

# EMAIL
1. **SMTP** serve para enviar email entre 2 clientes ou 2 servidores SMTP
2. **POP3** serve para enviar emails dos servers p/ clients
3. **IMAP** serve para administrar email folders

# Tecnologias de Rede diversas

**Domínios de Broadcast** são as áreas separadas por um roteador. **Intranet** é a parte da rede que só pode ser acessada internamente e **Extranet** é a parte da rede que pode ser acessada externamente. **Air Gap** é um isolamento físico do sistema, cabos, etc. 

**Para se autenticar na rede o Microsoft AD usa o protocolo LDAP**

## Ranges de IP Privados
1. 10.x.x.x
2. 172.16.x.x - 172.31.x.x
3. 192.168.x.x

## DNS

**DNSSEC previne DNS Cache Poison porque envia respostas digitalmente assinadas com certificado**

### Zonas de DNS
1. **A** : IPv4 Addresses
2. **AAA** : IPv6 Addresses
3. **MX** : Mail Servers (Sendo o servidor primário o com menor preferência)

## Evitando Loops
**STP ou Rapid STP** previne a rede de broadcast storm ou loops. Ele faz isso enviando BPDUs para detectar os loops e bloquear as portas que geram tráfego redundante.

# Firewalls
1. **Stateless** : Igual do BOCOM, configura as regras estáticas e o FW só obedece
2. **Statefull** : Muda de acordo com o tráfego da Rede
3. **Web Application Firewall** : É colocado entre o host server e o client para proteger a webapp de ataques diversos como até mesmo XSS
4. **NGFW** : Inspeção à nível de aplicação, podendo filtrar conteúdos de pacotes e bloquear determinadas URLs

# NAT
**Network Address Translation** é o protocolo que traduz IPs públicos e privados. Pode ser implementado através de Port Address Translation e pode ser:
1. **Dinâmico** : Múltiplos IP's públicos e múltiplos IP's privados, podendo balancear o tráfego para algum deles
2. **Estático** : Tradução de um IP público para múltiplos privados

# Proxy

1. **Transparent Proxy** : Não modifica a requisição recebida pelo Proxy
2. **Non Transparent Proxy** : Pode modificar a requisição ou filtrar a URL