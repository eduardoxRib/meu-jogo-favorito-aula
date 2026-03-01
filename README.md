# 🎮 Meu Jogo Favorito

Projeto colaborativo da aula de Git. Cada aluno vai adicionar o seu jogo favorito na lista usando Git e GitHub.

---

## 📋 O que você vai fazer

1. Configurar o Git na sua máquina
2. Gerar um token no GitHub para autenticação
3. Clonar este repositório
4. Adicionar o seu jogo no arquivo `jogos.js`
5. Fazer commit e push
6. Abrir um Pull Request

---

## 1. Configurando o Git pela primeira vez

Abra o terminal e rode:

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"
```

---

## 2. Gerando um Token no GitHub

O GitHub não aceita mais senha comum. Você precisa gerar um **token de acesso**.

1. Acesse [github.com](https://github.com) e faça login
2. Clique na sua foto no canto superior direito → **Settings**
3. No menu lateral, vá até **Developer settings** (bem no final)
4. Clique em **Personal access tokens** → **Tokens (classic)**
5. Clique em **Generate new token (classic)**
6. Em **Note**, escreva algo como `aula-git`
7. Em **Expiration**, escolha **7 days**
8. Marque a opção **repo**
9. Clique em **Generate token**
10. **Copie o token agora!** Ele só aparece uma vez.

> 💡 O token é uma sequência longa como `ghp_xK92mNzQwErT...`. Guarde em algum lugar seguro, pois você vai usá-lo como senha.

---

## 3. Clonando o repositório

```bash
git clone https://github.com/usuario/meu-jogo-favorito-aula.git
```

Entre na pasta:

```bash
cd meu-jogo-favorito-aula
```

---

## 4. Criando sua branch

Crie uma branch com o seu nome para não conflitar com o trabalho dos outros:

```bash
git checkout -b seu-nome
```

Exemplo:

```bash
git checkout -b joao-silva
```

---

## 5. Adicionando o seu jogo

Abra o arquivo `jogos.js` e adicione um novo objeto no array, seguindo o modelo:

```js
{
  foto: "https://link-da-capa-do-jogo.jpg",
  titulo: "Nome do Jogo",
  genero: "Gênero do jogo",
  pessoa: "Seu Nome"
},
```

> 💡 Para pegar o link da imagem: pesquise a capa do jogo no Google Imagens → clique com botão direito na imagem → **Copiar endereço da imagem**.

---

## 6. Salvando as alterações (commit)

```bash
git add jogos.js # Ou: git add .
git commit -m "Adiciona jogo favorito do <Seu Nome>"
```

---

## 7. Enviando para o GitHub (push)

```bash
git push origin seu-nome
```

O terminal vai pedir **usuário** e **senha**:

- **Usuário**: seu nome de usuário do GitHub
- **Senha**: o **token** que você gerou no passo 2 (não a senha da conta!)

---

## 8. Abrindo um Pull Request

1. Acesse o repositório no GitHub
2. Vai aparecer um aviso amarelo com a sua branch — clique em **Compare & pull request**
3. Escreva uma mensagem descrevendo o que você fez
4. Clique em **Create pull request**

Pronto! O professor vai revisar e fazer o merge. 🎉

---

## 🗂️ Estrutura do projeto

```
meu-jogo-favorito-aula/
├── index.html   # Página principal (não mexa aqui)
└── jogos.js     # ← Arquivo que você vai editar
```

---

## ❓ Dúvidas comuns

**O terminal não reconhece o comando `git`**
→ O Git não está instalado. Baixe em [git-scm.com](https://git-scm.com)

**Digitei a senha mas deu erro de autenticação**
→ Verifique se você usou o token e não a senha da conta

**Apareceu um conflito no merge**
→ Chama o professor, vamos resolver juntos!
