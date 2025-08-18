# Fluxo Completo de Git e GitHub (Primeiros Passos)

Este documento resume o fluxo básico de uso do Git para iniciar um projeto do zero e enviá-lo para o GitHub.

---

## 1. Iniciar um repositório local
```bash
git init
```
Cria uma pasta `.git` no projeto, transformando-o em um repositório Git.

---

## 2. Verificar o status
```bash
git status
```
Mostra os arquivos modificados, novos ou não rastreados.

---

## 3. Adicionar arquivos
```bash
git add .
```
Adiciona todos os arquivos novos e modificados à área de stage.  
Pode-se adicionar arquivos específicos também, por exemplo:
```bash
git add index.html
```

---

## 4. Criar o commit
```bash
git commit -m "Mensagem do commit"
```
Registra as alterações no histórico do repositório local.

---

## 5. Conectar ao repositório remoto
```bash
git remote add origin https://github.com/usuario/repositorio.git
```
Conecta o repositório local a um repositório remoto no GitHub.

---

## 6. Enviar alterações para o GitHub
```bash
git push -u origin main
```
Envia os commits locais para a branch `main` no GitHub.  
O parâmetro `-u` conecta sua branch local com a branch remota.

---

## 7. Próximas alterações (ciclo contínuo)
Sempre que fizer novas mudanças:
```bash
git add .
git commit -m "Mensagem explicando a alteração"
git push
```

---

## Resumo Visual do Fluxo
1. `git init` → Cria o repositório local  
2. `git add .` → Adiciona arquivos à área de stage  
3. `git commit -m "mensagem"` → Salva no histórico  
4. `git remote add origin ...` → Conecta ao GitHub  
5. `git push -u origin main` → Envia ao repositório remoto  

---

Com esse ciclo, você já consegue versionar projetos e enviar para o GitHub.
