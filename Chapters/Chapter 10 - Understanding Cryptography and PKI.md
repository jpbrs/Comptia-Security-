# Hashes

**Hash Colision** é quando mais de uma entrada produz a mesma saída do algoritmo de Hash. MD5 é altamente suscetível à colisão.

| Stream Cipher | Block Cipher |
| ---------- | --------- |
| Encripta Bit a Bit ou Byte a Byte | Encripta a cifra por bloco |

## Hashes vs Checksums

Hashes e Checksums são parecidos, mas enquanto hashes são maiores e mais seguros, checksums são pedaços menores de dados feitos para fazer verificações rápidas

## Algoritmos de Hashes

1. MD5 : 128 bits
2. SHA3(tem 0,1 e 2, mas são deprecated), mais seguro que o MD5
3. HMAC : É um algoritmo de Hash que, com uma chave secreta, adiciona aleatoriedade ao embaralhar as informações. Portanto, como possui uma PSK, garante não só integridade como também autenticidade. **Esse algoritmo é usado pelo IPSec e TLS**

## Ataques envolvendo Hashes

1. **Birthday Attacks** : Tenta produzir uma Hash Colision com outra password
2. **Pass the Hash** : Um replay attack que passa a Hash como senha
3. **Spraying Attacks** : Usa mesma senha para tentar logar em diversas contas diferentes, o que ajuda a evitar account lock
4. **Rainbow Tables** : Ataque que usa tabelas de Hash de centenas de GB para comparar quais senhas geram quais Hashes

## Salting Passwords

É uma técnica que adiciona alguns caracteres na senha antes de gerar a Hash da mesma(como se fossem pitadas de sal). É possível aumentar a complexidade mais ainda com técnicas de Key Streching como BCrypt

# Criptografia

**Crypto Diversity** é a técnica de usar uma variedade de técnicas criptográficas para garantir a segurança dos dados criptografados

## Chaves Simétricas

Exemplos:
1. **AES** 128, 192 ou 256 bits de chave com 128 bit blocks
2. **3DES** 64 bit block(Alternativa ao AES para limited resources)
3. **Blowfish** 64 bit blocks encription. Criado pelo Bruce Shneier para substituir o DES

# Certificates

**Certificate Authority** fornece uma Public Key em forma de Cert\
**Ephemeral Keys** são chaves públicas e privadas que mudam a cada sessão\
**Homomorphic Encryption** é um tipo de criptografia que permite manipular dados sem decriptá-los\
**S/MIME** é um dos padrões mais populares de assinatura digital e criptografia de emails\

## Protocolos para requisição de certificados

### CSR(Certificate Signing Request)

É a forma/protocolo padrão de se exigir um certificado. Primeiro se cria uma chave privada RSA para depois criar a pública, enviando-a assim por CSR para a CA.

### CRL(Certification Revocation List)

É uma lista de certificados inválidos identificados pelo Serial Number

### OSCP

Certificados podem estar expirados, não serem confiáveis ou serem revogados, dando o status de inválido. Esse status pode ser verificado pelo protocolo OSCP(Online Status Protocol). Com a técnica de Stapling do OSCP, pode-se conferir a validade de certificados, adicionando um timestamp de resposta OSCP e fazendo uma assinatura digital de resposta. 

## Tipos de Certificados

1. **Machine** : Designado a uma máquina
2. **User** : Designado a um usuário
3. **Email** : Para assinaturas digitais
4. **Code Signing** : Para assinar a integridade do Código
5. **Self-Signed** : Por Private CA
6. **Root** : Certificado Raiz do CA
7. **Wildcard** : Pode ser usado para múltiplos domínios com um mesmo root.( Por isso se usa *). Como *.google.com serve para account.google.com ou cloud.google.com
8. **SAN(Subjective Alternative Name)** : Usado para múltiplos domínios com nomes diferentes, mas com mesmo dono. Ex: android.com e java.com
9. **Domain Validation** : Valida quem é dono de um domínio

# Manipulação de Chaves Criptográficas

**Key Scrow** é o ato de guardar uma cópia da chave privada em um ambiente seguro\
**Public Key Pinning** é uma técnica que ajuda a mitigar ataques de personificação de certificados pois quando configurada corretamente em um servidor, se responde a uma HTTPS request com um cabeçalho extra contendo uma lista de hashes de public keys válidas usadas pelo site

