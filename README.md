<div align="center">
  
# 🖥️ DOCUMENTAÇÃO: PERMISSÃO DE ARQUIVOS NO LINUX
`Status: Online` | `Environment: Ubuntu 22.04 LTS` | `Security: Active`

![Banner Dark Tech](https://media4.giphy.com/media/v1.Y2lkPTc5MGI3NjExZW03c2c0NTNxemoyMHhhdDRvOWIxZ3pyY2Z1ZjVla2t6OXczcTA4aCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/utx4rJxu0MiGc/giphy.gif)

*"Otimizar o código, proteger a rede e torcer para o sudo não pedir a senha duas vezes."*


### 📂 1. A Tríade de Alvos
*No Linux, as permissões são divididas em três grupos, sempre nesta ordem:*

u (User): O dono do arquivo.
g (Group): O grupo que tem acesso.
o (Other): Todo o resto do mundo (quem não é dono nem do grupo).

### 🔢 2. A Linguagem dos Números (Octal)
*É a forma mais rápida de configurar o acesso. Cada permissão tem um peso:*

<img width="715" height="291" alt="image" src="https://github.com/user-attachments/assets/ff8ad932-30ac-4e8e-905c-4e8814d00625" />

