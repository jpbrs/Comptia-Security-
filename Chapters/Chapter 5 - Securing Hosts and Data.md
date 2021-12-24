# VM

## Tipos de VM
1. **Persistente** : Cada VM é personalizada para cada usuário
2. **Não Persistente** : VM volta ao estado original após o Logoff

## Vulnerabilidades de VM
1. **VM Escape** : Interagir com o Hypervisor de dentro da VM e ter acesso ao Host
2. **VM Sprawl** : Quando uma organização tem muitas VM's não administradas, ocupa mais processamento e é difícil manter com os patches atualizados

# Hardware

**SED**, Self-encryption Disk, encripta e decripta dados no drive automaticamente. Ele não possui senha por padrão, com um Opal-Compliant ele só desbloqueia com senha.\

**BIOS** é um Firmware(Software + Hardware) que provê as instruções básicas para iniciar or PC, como por exemplo checar a integridade do sitema e do Hardware, detectar o OS, etc.\

**UEFI** tem as mesmas funções da BIOS, mas funciona em discos maiores e é independente da CPU\

**TPM** é um pedaço de hardware na placa mãe que armazena as chaves criptograficas. Ele também armazena assinaturas digitais de arquivos de boot para conferir a integridade dos mesmos a cada vez que dá um boot, bloqueando o boot para proteger os drives nesse caso. TPM possui uma chave privada de RSA marcada eletronicamente no seu chip.\

**HSM** é um dispositivo para criar, armazenar e gerenciar chaves criptograficas de um sistema. Diferentemente do TPM, o HSM é removível.

# Cloud

1. **On-premise** : Empresa é dona de tudo
2. **Off-Premise** : CSP é dono de parte das coisas

## Tipos de Cloud
1. **Public** : Amazon, Microsoft, Google, etc.
2. **Private** : Cloud de alguma empresa que é dona de tudo
3. **Community** : Um grupo com os mesmos interesses cria uma Cloud
4. **Hybrid Cloud** : Cloud que reúne 2 ou mais características acima

## Tipos de Serviço
1. **SaaS** : Serviço de Software ou Aplicação
2. **Paas** : Plataforma com OS e softwares pré-configurados pela CSP
3. **IaaS** : Serviço de Hardware de Suporte de Hardware
4. **Xaas** : Anything as a Service, como DB, segurança, armazenamento, etc.

## Segurança na Cloud

**CASB** : Cloud Access Security Broker, uma ferramento ou serviço entre a rede da empresa e a Cloud para garantir a segurança do tráfego\
**NGSWG** : Next Generation Security Web Gateway, provê um serviço de proxy para os clientes como filtrar URL e geralmente são cloud-based

# Mobile

## Políticas Mobile em Empresas
1. Corporate Owned
2. BYOD
3. Choose Your Own Device(BYOD dentro de uma lista de devices permitidos)

**Mobile Device Management(MGM)** é uma política para dispositivos móveis\
**Unified Endpoint Management(UEM)** se certifica que os sistemas e patches estão atualizados\
**Para políticas BYOD, o ideal é rodar aplicações empresariais dentro de containers para proteger a aplicação**\
**Geofancing** é estabelecer um perímetro seguro de login geograficamente\
**Geotagging** é perigoso pois os metadados de uma foto podem indicar as coordenadas de, por exemplo, a casa de uma pessoa cuja foto foi tirada no local\
**Remote Wipe** é zerar o device de forma remota, como a Apple faz\
**Thetening e Mobile Hotspot** permitem que um dispositivo compartilhe sinal de internet\
**Jailbreak** é desbloquear um Iphone para aceitar Apps de non-authorized 3rd party\
**Rooting** é conseguir acesso de root num celular android\


