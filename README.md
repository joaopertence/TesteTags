# TesteTags

### Repositório para aprendizagem sobre o git:

* Git Flow
* Adição de tags 
* Realizar Merge
    * BranchA --> Master

### Comandos GitFlow:
Documentação: 
```
https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging
```

Cria Branch:
```
git checkout -b feature/branchA
```

Adicionar todas as modificações como stageds
```
git add .
```

Commitar
git commit -a -m 'commit inicial branch A'

### Mergear Branchs:

Documentação: 
```
https://www.atlassian.com/br/git/tutorials/using-branches/git-merge
```

Mergear alterações: 
```
branch A --> main
```

1º - Mudar para a branch que vai receber o merge:
```
git checkout main
```

2° - Atualizar todas asbranchs remotas:
```
git fetch --all
```

3° - Listar todas a branchs:
```
git branch -a
```

4° - Executar comando de merge (local):
```
git merge feature/branchA
```

... Resolver conflitos pelo vs code ...
```
Accept Current Change: Aceitar a mudança atual
Accept Incoming Change: Aceitar mudança recebida
Accept Both Change: Aceitar ambas as alterações
```

Finalizar realizando o commit com as alterações:
```
    git status
    git add .
    git commit -m '[MR] feature/branchA into main'
    git push
```

Exemplo Ilustrativo:

![exemplo](/images/fluxo_merge_exemplo.png).