# 🖥️ Kit de Sobrevivência - Terminal Git Bash

> Comandos mais importantes para uso diário em Git Bash, Linux e, em muitos casos, no WSL.

---

# ⭐ Comandos Essenciais

## Mostrar pasta atual

```bash
pwd
```

Mostra em qual diretório você está.

---

## Listar arquivos e pastas

```bash
ls
```

Lista arquivos e pastas.

### Mostrar arquivos ocultos

```bash
ls -a
```

### Mostrar detalhes

```bash
ls -l
```

---

## Entrar em uma pasta

```bash
cd nome-da-pasta
```

Exemplo:

```bash
cd projetos
```

---

## Voltar uma pasta

```bash
cd ..
```

---

## Ir para a pasta do usuário

```bash
cd ~
```

---

# 📂 Criar Arquivos e Pastas

## Criar pasta

```bash
mkdir projetos
```

---

## Criar várias pastas

```bash
mkdir html css javascript
```

---

## Criar arquivo vazio

```bash
touch index.html
```

---

## Criar vários arquivos

```bash
touch index.html style.css script.js
```

---

# 📋 Copiar

## Copiar arquivo

```bash
cp arquivo.txt copia.txt
```

---

## Copiar pasta

```bash
cp -r pasta pasta-copia
```

---

# 🚚 Mover

## Mover arquivo

```bash
mv arquivo.txt documentos/
```

---

# ✏️ Renomear

## Renomear arquivo

```bash
mv antigo.txt novo.txt
```

---

## Renomear pasta

```bash
mv pasta-antiga pasta-nova
```

---

# 🗑️ Remover

## Remover arquivo

```bash
rm arquivo.txt
```

---

## Remover pasta

```bash
rm -r pasta
```

---

## Remover pasta sem confirmação

```bash
rm -rf pasta
```

⚠️ Use com cuidado.

---

# 📖 Visualizar Arquivos

## Mostrar conteúdo

```bash
cat arquivo.txt
```

---

## Ler arquivos grandes

```bash
less arquivo.txt
```

Pressione:

* `q` para sair
* `↑` e `↓` para navegar

---

## Editar arquivo

```bash
nano arquivo.txt
```

Atalhos:

* `Ctrl + O` → Salvar
* `Ctrl + X` → Sair

---

# 🔍 Pesquisa

## Encontrar arquivo

```bash
find . -name "arquivo.txt"
```

---

## Procurar palavra em arquivo

```bash
grep "texto" arquivo.txt
```

---

## Procurar palavra em vários arquivos

```bash
grep -r "texto" .
```

---

# ⚙️ Git Essencial

## Verificar status

```bash
git status
```

---

## Adicionar alterações

```bash
git add .
```

---

## Criar commit

```bash
git commit -m "mensagem"
```

Exemplo:

```bash
git commit -m "Adicionado material de estudo"
```

---

## Enviar para GitHub

```bash
git push
```

---

## Baixar atualizações

```bash
git pull
```

---

## Ver histórico

```bash
git log
```

---

## Ver branches

```bash
git branch
```

---

## Criar branch

```bash
git branch nova-feature
```

---

## Trocar branch

```bash
git switch nova-feature
```

ou

```bash
git checkout nova-feature
```

---

## Juntar branch

```bash
git merge nova-feature
```

---

# 🖥️ Informações do Sistema

## Mostrar usuário

```bash
whoami
```

---

## Mostrar data e hora

```bash
date
```

---

## Mostrar processos

```bash
ps
```

---

# ⌨️ Atalhos do Terminal

| Atalho   | Função              |
| -------- | ------------------- |
| TAB      | Autocompletar       |
| ↑        | Comando anterior    |
| ↓        | Próximo comando     |
| Ctrl + C | Cancelar comando    |
| Ctrl + L | Limpar tela         |
| Ctrl + R | Pesquisar histórico |
| Ctrl + A | Início da linha     |
| Ctrl + E | Fim da linha        |

---

# 🔄 Equivalência Git Bash x CMD

| Git Bash | CMD      |
| -------- | -------- |
| ls       | dir      |
| pwd      | cd       |
| clear    | cls      |
| cp       | copy     |
| mv       | move     |
| rm       | del      |
| rm -r    | rmdir /s |
| cat      | type     |
| whoami   | whoami   |

Observação: o comando `touch` não possui equivalente nativo no CMD.

---

# 🎯 Kit de Sobrevivência

Se decorar apenas estes comandos, já consegue trabalhar na maioria dos projetos:

```bash
pwd
ls
cd
mkdir
touch
rm
cp
mv
cat
clear

git status
git add .
git commit -m "mensagem"
git push
git pull
```

---

# 📝 Dica de Memorização

Agrupe os comandos por função:

### Navegação

```bash
pwd
ls
cd
```

### Criação

```bash
mkdir
touch
```

### Manipulação

```bash
cp
mv
```

### Remoção

```bash
rm
```

### Visualização

```bash
cat
less
```

### Git

```bash
git status
git add .
git commit -m ""
git push
git pull
```

Aprenda os grupos, não os comandos isoladamente.
