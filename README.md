# Meu Segundo git
Repositório para apreender mexer com git e gitflow

...
## Comandos

Principais Comandos do GIT

...
### Branches

Para criar uma branch, use `git checkout -b prefixo/nome-da-branch`

Para mudar de branch, use `git checkout prefixo/nome-da-branch`

Para listar as branches, use `git branch`

E para apagar uma branch, use `git branch prefixo/nome-da-branch -D`

...
#### Atualizações

Para adicionar uma atualização, use `git add .`, onde `.` representa a pasta onde está atualmente (no terminal). Você pode adicionar tudo que estiver na pasta (e que foi modificado) ou pode adicionar arquivos  ou pastas especificos (`git add ./index.html`).

Para comitar as alterações adicionadas devemos execultar `git commit -m 'prefixo: descrição do commit` - importante que a descrição seja clara para facilitar futuras buscas no repositório, seja para achar uma funcionalidade ou um motivo de bug.

Para "empurrar" as atuaalizações para a origem, rode `git push origin prefixo/nome-da-branch`. Se for uma branch que só existe localmente, podera abrir uma PR.

Para "puxar" as atualizações da origem, rode `git pull origin prefixo/nome-da-branch`.

Para mergear uma PR já aprovada - via terminal - acesse a branch que deve receber a PR/Atualizações com `git checkout prefixo/nome-da-branch-que-recebe-a-pr`, rode um `git pull prefixo/nome-da-branch-que-recebe-a-pr` para garantir que está atualizada e, por fim, `git merge prefixo/nome-da-branch-da-PR`. Agora você tem as alterações localmente. Só falta jogar na origem (`git push origin prefixo/nome-da-branch-que-recebe-a-pr`).

