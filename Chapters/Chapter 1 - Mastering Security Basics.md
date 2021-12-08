# Security Controls
1. Managerial : Documentado, como políticas de Segurança
2. Operational : Para garantir que as operações do dia-a-dia respeitem a Política de Segurança
3. Technical : Hardware e Software

# Types of Control
1. Preventive : Previne que ocorra
2. Detective : Detecta quando ocorre
3. Corrective/Recovery : Como backups
4. Physical
5. Deterrent : Para desencorajar a ameaça
6. Compensating
7. Response : Incident response

**Cada medida de segurança pode combinar um Security Control com ou mais tipos**

## Windows Event Viewer
Possibilita ver todos os logs do windows. **Outro log management para windows é o NXLog**

## Syslog
Protocolo que explicita um formato de log e detalhes de transporte de logs. **Historicamente usou-se a porta UDP 514 ou TCP 6514** para isso.

## /var/log
Pasta de logs do linux que inclui:
1. /syslog : Logs do Systema
2. /messages : Mensagens de logs
3. /boot.log : Logs de Inicialização
4. /auth.log : Logs de logins
5. /Kern.log : Logs do Kernel
6. /httpd : Logs do Apache

![](permission.png)
