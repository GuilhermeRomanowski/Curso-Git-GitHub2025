# Curso Git & GitHub 2025

Fazendo curso iniciante para aprender a trabalhar com versionamento de código e repositórios remotos com GitHub. Utilizando blocos de notas juntamente com Readme. Sempre criar uma branch secundária e não trabalhar diretamente na main.

Testanto nova alteração com VSCode.

Fazendo novas alterações no VSCode, para primeira manutenção utilizando fluxo de trabalho conforme as branchs:
Main: Ambiente de produção
Develop: Ambiente de desenvolvimento (testar antes de fazer inclusão diretamente na Main)
Docs/Readme: Seguindo padrão de trabalho informando que essa branch será feita para alterar a documentação do arquivo Readme.

MAIN -> DEVELOP -> DOCS/README

Testando agora arquivos em .py ('Hello World')

--------------------------------------------------------------
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

## Documentação para tipos de branchs
1. docs: apenas mudanças de documentação;
2. feat: uma nova funcionalidade;
3. fix: a correção de um bug;
4. perf: mudança de código focada em melhorar performance;
5. refactor: mudança de código que não adiciona uma funcionalidade e também não corrigi um bug;
6. style: mudanças no código que não afetam seu significado (espaço em branco, formatação, ponto e vírgula, etc);
7. test: adicionar ou corrigir testes.

Fonte: (https://medium.com/prolog-app/nossos-padr%C3%B5es-de-nomenclatura-para-branches-e-commits-fade8fd17106)