# Termos novos
**Shadow IT** - Qualquer sistema não autorizado dentro de uma organização. Ex: Softwares baixados sem permissão\

**Command and Control** - Servidor que o bot herder irá controlar a botnet\

**Pottentially Unwanted Program** - PUPs são programas tipo o Baidu, que você baixa sem querer pois vem junto de algum outro software e faz da sua vida um inferno\

**File Integrity Monitors** - Usa hashes para checar e recalcular a integridade dos arquivos de tempos em tempos

**Cuckoo Sandbox** - Software Open Source que analisa arquivos em uma VM sandbox para classificar arquivos e URL's como maliciosos ou não

# Tipos de Malware

1. **Vírus**: Infecta uma aplicação e executa quando ela é executada. Tenta se replicar na máquina achando outras aplicações como hospedeiras
2. **Worm** : Malware que se replica pela rede
3. **Logic Bomb** : É um malware programado para ser executado após um evento específico, seja quando uma aplicação for executada no host ou quando um determinado dia/horário específico for atingido
4. **Trojan** : Malware que é instalado junto com um download de um software que a priori demonstrava ter alguma utilidade específica
5. **Remote Access Trojan(RAT)** : Permite que o Atacante controle o sistema infectado de forma remota
6. **Keylogger** : Hardware ou software projetado com o objetivo de gravar os dados produzidos pelo teclado
7. **Spyware** : Instalado sem o conhecimento do usuário, serve para monitorar as atividades do host
8. **Rootkit** : Um grupo de programas que atuam em Kernel level e que escondem o fato que o sistema foi comprometido
9. **Fileless Malware** : Malwares que não estão escritos em disco, mas sim em memória. Geralmente são scripts como PowerShell, Bash, Python, etc. que são injetados em aplicações populares como Java ou Adobe para serem executados juntamente à essas aplicações

# Engenharia Social

1. **Impersonation** : Fingir ser alguém, seja por email ou IP ou na vida real
2. **Shoulder Surfing** : Olhar por cima do ombro de alguém que esteja colocando uma senha ou escrevendo algo confidencial
3. **Hoaxes** : Mensagens para convencer o usuário de algo falso, como por exemplo para ele deletar a pasta sys32
4. **Tailgating** : Andar próximo a um usuário autorizado para passar por uma entrada restrida
5. **Mantrap** : Impede tailgating pois só permite uma pessoa por vez passar, é como se fosse uma sala com 2 portas, sendo que a segunda só abre quando a segunda fecha
6. **Dumpster Diving** : Buscar informações revirando lixo
7. **Watering Hole** : Descobrir quais sites são visitados pelos alvos e infectar esses sites com vírus para conseguir atingir os alvos indiretamente
8. **Typo Squatting** : Quando se aproveita de um domínio de URL malicioso que é muito parecido com outro site famoso. Ex: facebok, twiter, instagran, snapshat
9. **Invoice Scan** : O que fazem na English Live, encher seu saco com mensagens de voz alegando serem alguém que não são
10. **Credential Harvesting** : Buscar credenciais como criando páginas falsas com telas de login, etc.
11. **Gaslighting** : O termo vem do filme Gaslight, onde o marido tenta alegar que a sua esposa está com insanidade mental após alterar constantemente a luminosidade das lâmpadas de gás. Gaslighting é fazer a pessoa duvidar da própria sanidade.

## Engenharia Social Via Email ou Telefone/Celular

1. **Spam**
2. **Phishing e Spear Phishing** : Phising é jogar baits para pessoas cairem, e Spear Phishing é um Phishing direcionado a um público ou pessoa ao se personificar uma pessoa muito específica como o Tom do TI, o que pode ser impedido com assinaturas digitais dos remetentes
3. **Whaling** : Spear Phishing com foco em personificar altos executivos
4. **Vishing** : Phishing por voz
5. **SMSishing** : Phishing por SMS


# Threat Intelligence Sources

1. **Vulnerability Databases** : CVE, NVD, etc.
2. **TAXII** : Forma que deve ocorrer a troca de mensagens referentes à vulnerabilidades
3. **STIX** : Define que info de vulns uma organização pode compartilhar
4. **IOC, Darknet, Public/Private centers**
5. **Threat Maps** : Ver link(favoritado no PC)
6. **Repositórios** : Ver link(favoritado no PC)


