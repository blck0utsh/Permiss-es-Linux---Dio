<div align="center">
  
# 🖥️ DOCUMENTAÇÃO: PERMISSÃO DE ARQUIVOS NO LINUX
`Status: Online` | `Environment: Ubuntu 22.04 LTS` | `Security: Active`

![Banner Dark Tech](https://media4.giphy.com/media/v1.Y2lkPTc5MGI3NjExZW03c2c0NTNxemoyMHhhdDRvOWIxZ3pyY2Z1ZjVla2t6OXczcTA4aCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/utx4rJxu0MiGc/giphy.gif)

*"Otimizar o código, proteger a rede e torcer para o sudo não pedir a senha duas vezes."*


### 📂 1. A Tríade de Alvos
*No Linux, as permissões são divididas em três grupos, sempre nesta ordem:*

<img width="521" height="147" alt="image" src="https://github.com/user-attachments/assets/3e7dba54-f677-4bc6-82ad-6b130851ce36" />


### 🔢 2. A Linguagem dos Números (Octal)
*É a forma mais rápida de configurar o acesso. Cada permissão tem um peso:*

<img width="715" height="291" alt="image" src="https://github.com/user-attachments/assets/ff8ad932-30ac-4e8e-905c-4e8814d00625" />

### 🛠️ 3. Combinações Mortais
*Você soma os valores para dar o acesso final*
7 (4+2+1): Poder total (rwx).
6 (4+2): Ler e escrever (rw-).
5 (4+1): Ler e executar (r-x).
0: Sem acesso (---).

# Exemplo Clássico: chmod 755 arquivo
7 (Dono): Faz tudo.
5 (Grupo): Só lê e executa.
5 (Outros): Só lê e executa.

### ⌨️ 4. Comandos de Operação
chmod: Altera quem pode fazer o quê (as permissões).
chown: Altera quem é o dono do arquivo (troca a propriedade).
chgrp: Altera o grupo do arquivo.

## 💀 5. Dica de Red Team: O Perigo do 777
Nunca use chmod 777 em produção. Isso dá permissão de escrita para qualquer pessoa no sistema. É como deixar a porta da frente aberta com uma placa escrita "Pode entrar". No Red Team, encontrar um arquivo 777 é o primeiro passo para uma escalação de privilégios.

![Banner Dark Tech]([https://media4.giphy.com/media/v1.Y2lkPTc5MGI3NjExZW03c2c0NTNxemoyMHhhdDRvOWIxZ3pyY2Z1ZjVla2t6OXczcTA4aCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/utx4rJxu0MiGc/giphy.gif])
