# Permissões aplicadas

Ficheiro	Permissão	Justificação

 publico.txt	 644	          Permite leitura a todos, mas apenas o proprietário pode alterar o ficheiro.
 restrito.txt	 640	          Restringe o acesso a outros utilizadores, permitindo apenas leitura ao grupo.
 script.sh	 u+x	          Permite a execução do script apenas pelo proprietário, mantendo controlo de execução.


## Ambiente utilizado
WSL2 / Linux (Ubuntu)

## Utilizador e grupos
O utilizador atual foi identificado através dos comandos:

- `whoami` → mostra o nome do utilizador atual no sistema
- `id` → apresenta o UID, GID e grupos associados ao utilizador
- `groups` → lista os grupos aos quais o utilizador pertence

## Saída:

===== whoami =====
ubuntu

===== id =====
uid=1000(ubuntu) gid=1000(ubuntu) groups=1000(ubuntu),4(adm),24(cdrom),27(sudo),30(dip),46(plugdev),100(users)

===== groups =====
ubuntu adm cdrom sudo dip plugdev users


## Ficheiros criados

publico.txt -> ficheiro de acesso público com permissões de leitura para todos os utilizadores.
restrito.txt -> ficheiro com acesso limitado apenas ao proprietário e ao grupo.
script.sh -> script executável que imprime uma mensagem no terminal.

## Relação com o princípio do menor privilégio

O princípio do menor privilégio estabelece que cada utilizador ou processo deve ter apenas as 
permissões necessárias para executar as suas funções.

Neste exercício, foram aplicadas permissões restritas para evitar acessos desnecessários ou 
modificações indevidas. O ficheiro publico.txt mantém leitura pública controlada, o restrito.txt 
limita o acesso a utilizadores não autorizados, e o script.sh só pode ser executado pelo proprietário, 
reduzindo riscos de execução não autorizada ou alterações maliciosas.
