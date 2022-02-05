# Authentication Factors
1. Something You Have
2. Something You Know
3. Something You Are

**Para haver multi-factor authentication, é necessário que mais de um desses fatores sejam utilizados**

## Senhas
1. Complex Passwords são senhas com caractéres especiais
2. Senhas fortes são senhas complexas que possuem um determinado tamanho mínimo

# Tabela de Conhecimentos do Capítulo
| Tecnologia | Utilidade |
| ---------- | --------- |
| Password Vault | Gerenciador de senhas, como o do Chrome |
| Account Lockout | Bloquear a conta do usuário depois da tentativa N |
| HOTP e TOTP | São padrões open source para criar one-time passwords. Enquanto o HOTP não expira até ser usado, o TOTP expira a cada 30 segundos.
| PAM System | É um sistema que apenas concede determinados privilégios de forma temporária à uma determinada conta que explicitamente os requisitou. |
| Privillege Creep ou Permission Bleat | É quando o usuário acumula privilégios após mudar de área/tipo de conta. Uma account audit identificaria quando o Least Privillege não é seguido e detecta essa anomalia |
| Kerberos | Protocolo de autenticação em rede que usa criptografia simétrica para se autenticar no Windows AD ou Unix Realm. Ele usa um banco de dados e um KDC para criar tickets com timestamps, válidos por um determinado intervalo de tempo |
| Federation | Une privilégios de autenticação de 2 sistemas sem juntá-los. Para isso precisamos de um Federation Identity Management |
| OAuth | É um padrão de autorização entre websites que permite você usar uma conta como Gmail ou Facebook para realizar serviços no site |

**Exigir que administradores usem 2 contas, 1 com e 1 sem privilégios, dificulta que se tenha acesso de admin com ataques de escalação de privilégios**

# Access Controls
1. **Role-Based ou Role-BAC** : Separar por função/departamento
2. **Rule-Based ou Rule-BAC** : Baseado em permitir ou bloquear acesso segundo regras. Ex:Rule-BAC estático como ACL de Firewalls ou Dinâmico como IPS(Intrusion Prevention Systems)
3. **Discretionary ou DAC** : Um dono de arquivo que controla as permissões. Ex: Windows e Linux Files, todo arquivo tem um DACList que mostra a ACL de acesso
4. **Atribute-Based ou ABAC** : Usa políticas baseadas em atributos da conta para garantir acesso. É muito usada em SDN's. Ex: Atributo de Inspetor, TI, etc.
5. **MAC (Mandatory Access Control)** MAC (Mandatory Access Control) is an access control policy defined by system administrators.


**Conditional Access** é parecido com ABAC, mas as condições podem ser IP Location, MFA, Device Type/MAC, etc. Usada na Azure AD
