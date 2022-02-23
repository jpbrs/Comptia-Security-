# Jason Dion

1. Em criptografia, RC4 era o algoritmo simétrico de criptografia de fluxo mais usado no software e era utilizado nos protocolos mais conhecidos, como Secure Socket Layers e WEP
2. Cain & Abel (frequentemente abreviado para Cain) é uma ferramenta de recuperação de senha para Microsoft Windows. Ele pode recuperar muitos tipos de senhas usando métodos como sniffing de pacotes de rede, decifrando vários hashes de senhas, por meio do uso de métodos como ataques de dicionário, força bruta e ataques de análise de criptografia.[1] Os ataques de criptoanálise são feitos através de tabelas de arco-íris, que podem ser geradas com o programa winrtgen.exe, fornecido com o Cain & Abel
3. MSSP vem da sigla em inglês Managed Security Services Providers. São empresas que proveem serviços gerenciados de segurança para outras empresas, através de um SOC – Security Operations Center. 

## SMURF ATTACK

A Smurf attack scenario can be broken down as follows:

1. Smurf malware is used to generate a fake Echo request containing a spoofed source IP, which is actually the target server address.
2. The request is sent to an intermediate IP broadcast network.
3. The request is transmitted to all of the network hosts on the network.
4. Each host sends an ICMP response to the spoofed source address.
5. With enough ICMP responses forwarded, the target server is brought down.

## General Knowledge

1. If a user or system has configured their email accounts to require two-factor authentication (2FA) or multifactor authentication, then even if they enter their username and password correctly in the third-party email client, they will receive the "Invalid credentials" error message.
2. Application blocklisting is the most appropriate practice to implement to block a limited number of known programs. Application allow listing could be used to achieve this purpose, but it would require much more work and block every program not specifically allowed by the allow list or approve list policy
3. The purple team is made up of both the blue and red teams to work together to maximize their cyber capabilities through continuous feedback and knowledge transfer between attackers and defenders.
4. No contexto de redes de computadores, IP spoofing é um ataque que consiste em mascarar (spoof) pacotes IP utilizando endereços de remetentes falsificados.
5. PIV é person identification verification device, tudo que conseguir identificar uma pessoa como por exemplo Biometrics pode ser PIV
6.  Diretiva de Grupo ou Group Policy (GPO) é uma funcionalidade da família de sistemas operacionais Microsoft Windows NT. É um conjunto de regras que controlam o ambiente de trabalho de contas de usuário e contas de computador. Ela fornece o gerenciamento e configuração centralizados de sistemas operacionais, aplicativos e configurações dos usuários em um ambiente Active Directory. Em outras palavras, a Diretiva de Grupo controla em parte o que os usuários podem ou não fazer em um sistema de computador
7. Banner Grabbing é uma técnica usada para obter informações sobre um sistema de computador em uma rede e os serviços em execução em suas portas abertas.
8. One-time pad (OTP), em português cifra de uso único ou chave de uso único, é uma técnica de criptografia que não pode ser quebrada se utilizada corretamente. Consiste num algoritmo em que o purotexto é combinado, caractere por caractere, a uma chave secreta aleatória que para isso deve ter, no mínimo, o mesmo número de caracteres do purotexto. Para garantir que a criptografia seja imperscrutável, a chave só deve ser usada uma única vez, sendo imediatamente destruída após o uso
9. IP Theft é INTELLECTUAL PROPERTY THEFT
10. **A Golden Ticket attack** is when an attacker has complete and unrestricted access to an entire domain — all computers, files, folders, and most importantly, the access control system itself. A golden ticket is a Kerberos ticket that can grant other tickets in an Active Directory environment
11. **Double File Extension**. Adversaries may abuse a double extension in the filename as a means of masquerading the true file type. A file name may include a secondary file type extension that may cause only the first extension to be displayed (ex: File. txt.exe may render in some views as just File. txt )
12. **Dereferencing** é quando um ponteiro é desreferenciado e aponta para outra parte da memória. This is where the programmer is dereferencing a portion of memory that’s being used by that application, except in this case there’s nothing at that memory address to dereference and the application crashes.
13. In both cases (trusted boot and the measured boot), the basic flow starts with the TPM performing a measurement of the BIOS/EFI layer. After measuring the BIOS/EFI layer, the next layer (firmware) is measured. In this case, the resulting hash is combined with the previous hash (which was stored in the PCR slot) and then also stored in a PCR slot. The process continues until all the layers involved in the process have been measured and the hashes' results have been stored.
14. Iris recognition looks at the unique patterns in the iris. Because the iris is visible, the process of enrolling and identifying people is simple. To enroll an iris or irides, a person stands at distance from the iris recognition camera which uses an infrared camera (similar to a regular camcorder) to take a digital photo of the iris. A retinal scan looks at the complex network of vessels that supply the retina with blood. A special scanning device is used to shoot a beam of light into the eye. To enroll, a person must be positioned very close to the scanner – much closer than for iris recognition.
16. WPA (Wi-Fi Protected Access) é um protocolo de comunicação via rádio. **É um protocolo WEP melhorado.** Também chamado de WEP2, ou TKIP (Temporal Key Integrity Protocol), essa primeira versão do WPA (Wi-Fi Protected Access) surgiu de um esforço conjunto de membros da Wi-Fi Aliança e de membros do IEEE, empenhados em aumentar o nível de segurança das redes sem fio ainda no ano de 2003, combatendo algumas das vulnerabilidades do WEP.
17. Combining the dictionary and brute force methods into a single tool is known as a hybrid password cracking approach.
18. Attribute-based access control (ABAC) provides the most detailed and explicit type of access control over a resource because it is capable of making access decisions based on a combination of subject and object attributes, as well as context-sensitive or system-wide attribute
19. Pass the Hash (PtH) is the process of harvesting an account's cached credentials when the user logs in to a single sign-on (SSO) system. This would then allow the attacker to use the credentials on other systems, as well

## Federations

Possuem Identity Providers e Service Providers ou Request Provider Authentication.

SAML is a solution for providing single sign-on (SSO) and federated identity management. It allows a service provider (SP) to establish a trust relationship with an identity provider (IdP) so that the SP can trust the identity of a user (the principal) without the user having to authenticate directly with the SP



## Em um caso onde um funcionário da empresa tem sua Workstation agindo estranhamente

Isolation of Connor’s computer by deactivating the port on the switch should be performed instead of just unplugging the computer. This would guarantee that Connor won’t just plug the computer back into the network as soon as you leave his desk.

## Caso onde o Database é infectado e a rede não

Como a rede é uma parte critica da organização, deve ser feito um monitoramento dela pela analise forense para assegurar que tudo está seguro. Since the database server is part of a critical production network, it is important to work with the business to time the remediation period to minimize productivity losses. You can immediately begin to capture network traffic since this won't affect the database server or the network (least intrusive) while scheduling a period of downtime in which to take a forensic image of the database server's hard drive. All network captures and the hard drive should be maintained under the chain of custody if needed for criminal prosecution or civil action after remediation. The server should be remediated and brought back online once the hard drive image has been created.

# Limpeza de Disco

1. Hard drive degaussing is a process whereby powerful magnets are used to scramble all data stored on magnetic media such as hard disk drive (HDD) technology.
2. A forensic disk controller or hardware write-block device is a specialized type of computer hard disk controller made for the purpose of gaining read-only access to computer hard drives without the risk of damaging the drive's contents.
3. Disk Wipe is a free software that does so, it wipes the disk using one of predefined advanced algorithms, by overwriting the existing disk data with a new
4. O Zero Fill grava zeros em cada setor de dados até a capacidade completa da unidade e limpa a maioria dos defeitos.
5. The process of permanently erasing data from the hard disk by overwriting so that no data can be recovered from it by any means is called hard disk sanitization.

In a cryptographic erase (CE), the storage media is encrypted by default. The encryption key itself is destroyed during the erasing operation. CE is a feature of self-encrypting drives (SED) and is often used with solid-state devices. Cryptographic erase can be used with hard drives, as well. Zero-fill is a process that fills the entire storage device with zeroes. For SSDs and hybrid drives, zero-fill-based methods might not be reliable because the device uses wear-leveling routines in the drive controller to communicate which locations are available for use to any software process accessing the device. For example, performing a cryptographic erasure (CE) would sanitize and purge the drives' data without harming the drives themselves. Clearing them leaves the possibility that some tools would allow data recovery.

# Vazamento de Emails da compania fazendo Phishing

 You should first request a copy of one of the spam messages, including the full email header. By reading through the full headers of one of the messages, you can determine where the email originated from, whether it was from your email system or external, and if it was a spoofed email or a legitimate email

## Endereços Locais

1. 10.0.0.0 – 10.255.255.255
2. 172.16.0.0 – 172.31.255.255
3. 192.168.0.0 – 192.168.255.255	

# RTO vs RPO

Recovery time objective (RTO) is when an individual IT system may remain offline following a disaster. This represents the amount of time it takes to identify a problem and then perform recovery (restore from backup or switch in an alternative system, for instance). Recovery point objective (RPO) is the amount of data loss that a system can sustain, measured in time. That is, if a virus destroys a database, an RPO of 24 hours means that the data can be recovered (from a backup copy) to a point not more than 24 hours before the database was infected

Ps: Mean time to repair (MTTR) is a measure of the time taken to correct a fault to restore the system to full operation. **Não necessariamente tem a ver com desastres**

# Políticas de Proteção de Dados

1. HIPAA (Health Insurance Portability and Accountability Act) é um conjunto de normas que organizações de saúde norte-americanas devem cumprir para proteger as informações. Em português, seria Lei de Portabilidade e Responsabilidade de Seguro Saúde.
2. SOX é o apelido dado para a lei Sarbanes-Oxley. Também conhecida como SOXO ou Sarbox, ela é responsável por aperfeiçoar a governança corporativa e as prestações de contas destas corporações como, por exemplo, a divulgação de informações sobre o balanço patrimonial, despesas e receitas, a fim de garantir o compliance
3. A Lei Gramm-Leach-Bliley (GLBA) é uma lei dos EUA que reformou o setor de serviços financeiros, permitindo que bancos comerciais e de investimento, empresas de valores mobiliários e empresas de seguros se consolidem e abordam as preocupações sobre a proteção da privacidade do consumidor
4. A Lei de Privacidade e Direitos Educacionais da Família (FERPA) é uma lei federal dos EUA que protege a privacidade dos registros educacionais dos alunos, incluindo informações de identificação pessoal e diretório
5. FISMA defines a framework for managing information security that must be followed for all information systems used or operated by a U.S. federal government