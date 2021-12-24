# IDS 

## Tipos
1. **Host-Based** : Instalado em servidores e pode detectar atividade maliciosa que anti-virus não conseguiram
2. **Network-Based** : Instalado em equipamentos de rede como switches, roteadores e Firewalls. Só detecta anomalias em hosts específicos se estas alterarem o tráfego da rede de forma significativa. **Só funciona para tráfego não criptografado**

## Metodologia
1. **Signature Based** : IDS que se baseia num Banco de Dados de vulnerabilidades e compara os comportamentos dos hosts com o das vulnerabilidades
2. **Heuristic/Behavioral** : IDS que a partir de uma Baseline, um conjunto de dados que equivalem a um tráfego sem anomalias, consegue detectar anomalias que alteram o statu quo da rede. Útil para detectar Zero Days. PS: Quando se instala um serviço e esse serviço altera a normalidade do tráfego, é necessário alimentar o IDS com uma nova *baseline*.

# Honey Stuff

1. Honeypot -> Dispositivos vulneráveis para serem infectados por malwares que eventualmente serão estudados
2. Honeyfiles -> Mesma ideia de honeypot, mas com arquivos. Ex: Arquivo password.txt com log para saber quando alguém tentou acessa-lo
3. Honeynet -> Grupo de Honeypot em uma rede separada

# WiFi

1. Ter o SSID padrão pode dar pistas sobre o equipamento. Ex: TP-Link, Linksys
2. MAC Filtering pode ser bypassado ao se alterar o endereço MAC dos pacotes para de algum MAC da ACL observado por Sniffing. O nome disso é MAC Spoof/Clonning

**Site Survey** é o mapeamento das redes Wifi no local para identificar quais faixas de frequência são as mais usadas.\
**Footprinting** é quando criamos um diagrama dos AP's do local

## WPA2
**WPA e WEP** estão deprecated, atualmente se usa WPA2 que usa criptografia AES e CCMP.

### Modes
1. **Pre-Shared Key** : Usuário acessa a rede WPA2 com uma senha. Provê autorização, mas não autenticação.
2. **Enterprise Mode** : Usa Radius p/ fornecer autenticação com o protocolo **802.1X**. É necessário o IP do Radius Server, a Radius Port e o Shared Secret para se autenticar na rede.

**WPA3** usa Diffie-Helman ao invés de Pre-Shared Key

## Autenticação com 802.1X

**802.1X** provê port-based authentication para que apenas pessoas autorizadas se conectem

1. **EAP** : Forma de 2 servidores criarem uma chave segura de criptografia chamada PMK.
2. **PEAP** : EAP usando TLS, requer certificado digital no **Server** para funcionar
3. **EAP-FAST** : EAP Light Weight, suporta certificados digitais como opicionais
4. **EAP-TLS** : Mesma coisa que o PEAP, requer um certificado 802.1X tanto no Client, quanto no **Server** para funcionar.

Uma alternativa barata aos servers 802.1X que são usados no Enterprise mode do WPA2 é o **Captive Portal**. O Captive Portal força o cliente que usa a internet via web-browser a completar um processo específico antes de logar na rede, como aceitar uma política, colocar quarto do hotel ou usuário da nota fiscal(Starbucks). 

## Wireless Threats

**War Flying e War Driving** é a busca ativa de redes Wifi dirigindo ou voando

### WIFI Threats

**WPS** quando ligado é uma ameaça à rede, visto que ele cria um PIN que permite que o usuário se autentique na rede WPA-2, mas é sucetível à Brute Force.

1. **Disassociation Attack** : Mandar frames de desassociação para desonectar os dispositivos da rede wifi. Parecido com o Wifi-Deauther
2. **Evil Twin** : AP com mesmo SSID para roubar os dados dos usuários que acessam a rede wifi. Tipo o Wifi falso do metrorio.
3. **Initialization Vector Attack** : Alguns protocolos combinam a chave da Rede com Initialization Vectors(IV), o ataque descobre o IV antes dessa combinação para conseguir decriptar os protocolos utilizados

### Bluetooth

1. **Bluejacking** : Envia mensagens para o celular invadido
2. **Bluesnarffing** : Acessa aos dados do celular como contatos e mensagens
3. **Bluebugging** : Instala um Backdoor no Celular

# VPN

É comum deixar o servidor de VPN de uma rede privada na DMZ para ficar visível na internet, e daí se autenticam via RADIUS ou LDAP. O tráfego da VPN geralmente tem o tunelamento encriptado com o protocolo SSTP, que roda na porta 443 para evitar problemas com firewalls.

## Tipos de VPN

1. Split Tunnel : Administrador configura qual tráfego será encriptado e passará pelo server
2. Full Tunnel : Todo tráfego que passa pelo servidor é tunelado.
3. Site-to-Site VPN : Quando 2 servidores de VPN em localizações diferentes criam um túnel. Ex: 2 escritórios de uma empresa, cada um com a própria VPN

**L2TP** é o protocolo usado para transportar os pacotes do tráfego VPN na 2a camada do modelo OSI em tunelamento, **mas não encripta os pacotes, para isso serve o IPSec**

## NAC

**NAC** permite que a VPN cheque para ver se o computador tem os requisitos mínimos para conexão, como por exemplo algum Antivirus. Ele inspeciona o PC e só permite que ele se conecte caso passa na inspeção.\

Existem dois tipos de NAC:

1. **Com agentes** : Instalados no dispositivo, sendo permanenteme ou temporariamente
2. **Sem agentes** : Não é instalado, tudo é feito de forma remota

## Autenticação em VPN

### Descentralizada
1. **PAP** : Password Authentication Protocol, envia senha em texto plano
2. **CHAP** : Challenge Handshake Authentication Protocol, usa chave simétrica e um nonce dado pelo server para encriptar os dados de autenticação.
### Centralizada
1. **RADIUS** : Pode ser usado com UDP ou TCP, só encripta a senha por padrão, mas pode encriptar todo o processo de autenticação. Usado para centralizar a autenticação em diversos servidores VPM
2. **TACACS+** : Encripta todo o processo de autenticação, interage com Kerberos e além disso serve para acessar equipamentos de rede como switches e roteadores











