# Curso TMW Git & GitHub 2025

Um curso para iniciantes aprenderem a trabalhar com versionamento de código e repositórios remotos com GitHub.

Além disso, vamos trabalhar com GitFlow ao final do curso e Visual Studio Code.

Confira tudo o que temos no nosso YouTube. É gratis! Segue o link:

[Curso Git 2025](https://youtube.com/@teomewhy)

Além do nosso YouTube, se ligue no nosso site e agenda para ficar por dentro de tudo que vai rolar em 2025.

Conheça nosso site: [teomewhy.org](https://teomewhy.org/schedule)

Apoie nosso projeto no [Apoia-se](apoia.se/teomewhy)

## Fluxo de trabalho Git local

01. git checkout -b <nova-branch>
02. cria ou atualiza arquivos
03. git status
05. git add *arquivos*
06. git status
07. git commit -m "minha mensagem"
08. git checkout main
09. git merge nova_branch

## Fluxo de trabalho GitHub <> Local (projeto próprio ou da sua empresa)
01. git clone <endereco do projeto>
02. git checkout -b <nova_branch>
03. alterações de arquivos
04. git status
05. git add *arquivos*
06. git status
07. git commit -m "nova mensagem"
08. git push origin <nova_branch>
09. abrir Pull request no GitHub para main
10. excluir <nova_branch> origin
11. git checkout main
12. git branch -D <nova_branch>

## Fluxo de trabalho GitHub <> Local (projetos open-source)
01. Fork do projeto para seu próprio github
02. git clone <endereco do projeto fork>
03. git checkout -b <nova_branch>
04. alterações de arquivos
05. git status
06. git add *arquivos*
07. git status
08. git commit -m "nova mensagem"
09. git push origin <nova_branch>
10. abrir Pull request no GitHub da branch fork para a main do projeto original
11. excluir <nova_branch> origin
12. git checkout main
13. git branch -D <nova_branch>

----

O nosso padrão
Branches
Nomes de branches são compostos de 3 partes:

1 — type ou categoria do branch. Os types podem ser os seguintes:

- docs: apenas mudanças de documentação;

- feat: uma nova funcionalidade;

- fix: a correção de um bug;

- perf: mudança de código focada em melhorar performance;

- refactor: mudança de código que não adiciona uma funcionalidade e também não corrigi um bug;

- style: mudanças no código que não afetam seu significado (espaço em branco, formatação, ponto e vírgula, etc);

- test: adicionar ou corrigir testes.

2 — o que o branch faz em si

3 — Código da tarefa no Jira. Ex.: PL-123.

Exemplos de alguns nomes de branches que podem existir em nossa aplicação:

- feat-cadastro-veiculos-PL-123
- refactor-edicao-colaboradores-PL-355
- fix-busca-checklists-PL-232

git commit -m "test: add test for create product automation"
git commit -m "feat: implement tracking product service"
git commit -m "refactor: change return log pattern"
git commit -m "style: change function param for objects"
git commit -m "fix: remove getPayment() wrong attribute"
git commit -m "chore: add no-undef rule in eslintrc.json"
git commit -m "docs: add technologies list in readme"
git commit -m "style: remove all blank spaces"
git commit -m "perf: change looping for parallel execution"
git commit -m "build: remove moment.js dependency"
git commit -m "build: add date-fns npm dependency"
git commit -m "revert: back to a215868 commit"