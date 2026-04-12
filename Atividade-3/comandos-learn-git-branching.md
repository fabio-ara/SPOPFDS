# Atividade 3 — Learn Git Branching

## Main

### 1 Sequência introdutória

#### 1.1 Introdução aos commits no Git
```bash
git commit
git commit
```

#### 1.2 Branches no Git
```bash
git branch bugFix
git checkout bugFix
```

#### 1.3 Merge no Git
```bash
git branch bugFix
git checkout bugFix
git commit
git checkout main
git commit
git merge bugFix
```

#### 1.4 Introdução ao rebase
```bash
git checkout -b bugFix
git commit
git checkout main
git commit
git checkout bugFix
git rebase main


```

### 2 Acelerando

#### 2.1 Solte a sua cabeça
```bash
git checkout C4
```

#### 2.2 Referências relativas (^)
```bash
git checkout C4^
```

#### 2.3 Referências relativas #2 (~)
```bash
git checkout HEAD~1
git branch -f main C6
git branch -f bugFix HEAD~1
```

#### 2.4 Revertendo mudanças no Git
```bash
git reset local^
git checkout pushed
git revert pushed
```

### 3 Movendo trabalho por aí

#### 3.1 Introdução ao cherry-pick
```bash
git cherry-pick C3 C4 C7
```

#### 3.2 Introdução ao rebase interativo
```bash
git rebase -i HEAD~4
```

### 4 Sortidos

#### 4.1 Pegando um único commit
```bash
git checkout main
git cherry-pick C4
```

#### 4.2 Malabarismo com commits
```bash
git rebase -i HEAD~2
git commit --amend
git rebase -i HEAD~2
git branch -f main HEAD
```

#### 4.3 Malabarismo com commits #2
```bash
git checkout main
git cherry-pick C2
git commit --amend
git cherry-pick C3
```

#### 4.4 Tags no Git
```bash
git tag v0 C1
git tag v1 C2
git checkout v1
```

#### 4.5 Git Describe
```bash
git commit
```

### 5 Temas avançados

#### 5.1 Fazendo mais de 9000 rebases
```bash
git rebase main bugFix
git rebase bugFix side
git rebase side another
git rebase another main
```

#### 5.2 Múltiplos pais
```bash
git branch bugWork C2
```

#### 5.3 Espaguete de branches
```bash
git rebase main one
git rebase -i C1
git rebase main two
git rebase -i C1
git branch -f three C2
```

## Remote

### 6 Push & Pull - repositórios remotos no Git!

#### 6.1 Introdução à clonagem
```bash
git clone
```

#### 6.2 Branches remotos
```bash
git commit
git checkout o/main
git commit
```

#### 6.3 Git Fetch
```bash
git fetch
```

#### 6.4 Git Pull
```bash
git pull
```

#### 6.5 Simulando trabalho em equipe
```bash
git clone
git fakeTeamwork 2
git commit
git pull
```

#### 6.6 Git Push
```bash
git commit
git commit
git push
```

#### 6.7 Histórico divergente
```bash
git clone
git fakeTeamwork
git commit
git pull --rebase
git push
```

#### 6.8 Main bloqueado
```bash
git reset --hard o/main
git checkout -b feature C2
git push
```

### 7 Até a origin e além -- repositórios remotos avançados!

#### 7.1 Push Main!
```bash
git fetch
git rebase o/main side1
git rebase side1 side2
git rebase side2 side3
git rebase side3 main
git push
```

#### 7.2 Merge com remotos
```bash
git checkout main
git pull
git merge side1
git merge side2
git merge side3
git push
```

#### 7.3 Seguindo remotos
```bash
git checkout -b side o/main
git commit
git pull --rebase
git push
```

#### 7.4 Parâmetros do git push
```bash
git push origin main
git push origin foo
```

#### 7.5 Parâmetros do git push -- expandido
```bash
git push origin foo:main
git push origin main^:foo
```

#### 7.6 Parâmetros do fetch
```bash
git fetch origin foo:main
git fetch origin main^:foo
git checkout foo
git merge main
```

#### 7.7 Origem vazia
```bash
git push origin :foo
git fetch origin :bar
```

#### 7.8 Parâmetros do pull
```bash
git pull origin bar:foo
git pull origin main:side
```
