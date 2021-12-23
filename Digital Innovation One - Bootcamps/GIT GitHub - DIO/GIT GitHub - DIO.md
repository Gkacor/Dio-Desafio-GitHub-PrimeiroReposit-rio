# GIT/GitHub - DIO

Created: December 8, 2021 1:55 AM
Programação: GitHub
Reviewed: No

# Git e GitHub

O que é?

Git é o sistema de distribuição de código utilizado globalmente.

GitHub é o site onde o conteúdo é agrupado e distribuído, podendo ser modificado se colocado como público.

Para enviar os arquivos para o GitHub é necessário fazer um "commit". Exemplo:

!["Commitando" arquivos.](GIT%20GitHub%20-%20DIO%202e4faa2d3b1b42929acff4b28d8c1e86/Untitled.png)

"Commitando" arquivos.

- Para conferir o que tem na pasta: "ls"
- Para entrar nas pastas: "cd"
- Para recuar uma pasta: "cd .."
- Para criar uma nova pasta: "mkdir nomedapasta"
- Para mover o arquivo: "mv nomedoarquivo ./pasta/"
- Tab para completar.

### Stages

Existem quatro estágios do arquivo: 

- Untracked: Está "quieto", GIT não tem conhecimento.
- Unmodified: Não modificado, quando "commitado" volta para esse estágio.
- Modified: Modificado.
- Staged: Em modificação.

### Enviando pasta para o GitHub:

- git clone "linkdorepositório" -para clonar o repositório.
- git status - verifica com o que está mexendo, se existem pasta novas ou algo para "commitar".
- git add . - adiciona todos os arquivos.
- git commit -m "mensagemquequiser"
- git status novamente para conferir.
- git push origin main -main é a branch com que estamos mexendo, o "push" envia para a nuvem/github.

Exemplo:

```jsx
gkaco@DESKTOP-6BAMRS5 MINGW64 /c/Workspaceprog/DIO
$ git clone https://github.com/Gkacor/Dio-Desafio-GitHub-PrimeiroReposit-rio.git
Cloning into 'Dio-Desafio-GitHub-PrimeiroReposit-rio'...
remote: Enumerating objects: 6, done.
remote: Counting objects: 100% (6/6), done.
remote: Compressing objects: 100% (4/4), done.
remote: Total 6 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (6/6), done.

gkaco@DESKTOP-6BAMRS5 MINGW64 /c/Workspaceprog/DIO
$ cd Dio-Desafio-GitHub-PrimeiroReposit-rio/

gkaco@DESKTOP-6BAMRS5 MINGW64 /c/Workspaceprog/DIO/Dio-Desafio-GitHub-PrimeiroReposit-rio (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

gkaco@DESKTOP-6BAMRS5 MINGW64 /c/Workspaceprog/DIO/Dio-Desafio-GitHub-PrimeiroReposit-rio (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

gkaco@DESKTOP-6BAMRS5 MINGW64 /c/Workspaceprog/DIO/Dio-Desafio-GitHub-PrimeiroReposit-rio (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

gkaco@DESKTOP-6BAMRS5 MINGW64 /c/Workspaceprog/DIO/Dio-Desafio-GitHub-PrimeiroReposit-rio (main)
$ status
bash: status: command not found

gkaco@DESKTOP-6BAMRS5 MINGW64 /c/Workspaceprog/DIO/Dio-Desafio-GitHub-PrimeiroReposit-rio (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

gkaco@DESKTOP-6BAMRS5 MINGW64 /c/Workspaceprog/DIO/Dio-Desafio-GitHub-PrimeiroReposit-rio (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Estudos/

nothing added to commit but untracked files present (use "git add" to track)

gkaco@DESKTOP-6BAMRS5 MINGW64 /c/Workspaceprog/DIO/Dio-Desafio-GitHub-PrimeiroReposit-rio (main)
$ git add .

gkaco@DESKTOP-6BAMRS5 MINGW64 /c/Workspaceprog/DIO/Dio-Desafio-GitHub-PrimeiroReposit-rio (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   Estudos/notas.txt

gkaco@DESKTOP-6BAMRS5 MINGW64 /c/Workspaceprog/DIO/Dio-Desafio-GitHub-PrimeiroReposit-rio (main)
$ git commit -m "Adicionando notas e estudos"
[main eb7f895] Adicionando notas e estudos
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 Estudos/notas.txt

gkaco@DESKTOP-6BAMRS5 MINGW64 /c/Workspaceprog/DIO/Dio-Desafio-GitHub-PrimeiroReposit-rio (main)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

gkaco@DESKTOP-6BAMRS5 MINGW64 /c/Workspaceprog/DIO/Dio-Desafio-GitHub-PrimeiroReposit-rio (main)
$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (4/4), 328 bytes | 328.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Gkacor/Dio-Desafio-GitHub-PrimeiroReposit-rio.git
   6aa2e94..eb7f895  main -> main

gkaco@DESKTOP-6BAMRS5 MINGW64 /c/Workspaceprog/DIO/Dio-Desafio-GitHub-PrimeiroReposit-rio (main)
$
```