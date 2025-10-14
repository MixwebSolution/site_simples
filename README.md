# 🧱 Introdução ao HTML

## 1. O que é HTML?

O **HTML (HyperText Markup Language)** é a linguagem de marcação usada para **estruturar páginas da web**.
Ela **não é uma linguagem de programação**, mas sim uma forma de **organizar o conteúdo** — como textos, imagens, links, tabelas e formulários.

Um documento HTML é formado por **tags (marcadores)** que informam ao navegador o papel de cada parte do conteúdo.

---

## 🏗️ 2. Estrutura básica de um documento HTML

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Minha Primeira Página</title>
</head>
<body>
    <h1>Olá, mundo!</h1>
    <p>Bem-vindo à minha primeira página HTML.</p>
</body>
</html>
```

### 🧾 Explicando:

* `<!DOCTYPE html>` → define o tipo de documento (HTML5).
* `<html>` → tag raiz, envolve todo o conteúdo.
* `<head>` → contém informações não visíveis (metadados, título, estilos etc.).
* `<title>` → define o título da aba do navegador.
* `<body>` → parte visível da página (textos, imagens, links etc.).

---

## 📝 3. Tags de texto

| Tag                | Função                                 | Exemplo                        |
| ------------------ | -------------------------------------- | ------------------------------ |
| `<h1>` a `<h6>`    | Títulos e subtítulos (níveis de 1 a 6) | `<h2>Subtítulo</h2>`           |
| `<p>`              | Parágrafo                              | `<p>Este é um parágrafo.</p>`  |
| `<br>`             | Quebra de linha                        | `Linha 1<br>Linha 2`           |
| `<hr>`             | Linha horizontal                       | `<hr>`                         |
| `<b>` / `<strong>` | Negrito (semântico com `<strong>`)     | `<strong>Importante!</strong>` |
| `<i>` / `<em>`     | Itálico (semântico com `<em>`)         | `<em>Palavra em destaque</em>` |
| `<u>`              | Sublinhado                             | `<u>Texto sublinhado</u>`      |
| `<mark>`           | Texto marcado                          | `<mark>Texto destacado</mark>` |
| `<small>`          | Texto menor                            | `<small>Letra pequena</small>` |

### Exemplo:

```html
<h1>Título Principal</h1>
<p>Esse é um <strong>parágrafo</strong> com <em>ênfase</em> e <mark>destaque</mark>.</p>
```

---

## 🔗 4. Links e imagens

| Tag     | Função            | Exemplo                                             |
| ------- | ----------------- | --------------------------------------------------- |
| `<a>`   | Cria um link      | `<a href="https://google.com">Ir para o Google</a>` |
| `<img>` | Mostra uma imagem | `<img src="foto.jpg" alt="Descrição da imagem">`    |

### Exemplo:

```html
<a href="https://www.exemplo.com">Visitar site</a><br>
<img src="logo.png" alt="Logo do site" width="200">
```

---

## 🧱 5. Listas

| Tipo               | Tag                    | Exemplo                                                |
| ------------------ | ---------------------- | ------------------------------------------------------ |
| Lista não ordenada | `<ul>` + `<li>`        | `<ul><li>Item 1</li><li>Item 2</li></ul>`              |
| Lista ordenada     | `<ol>` + `<li>`        | `<ol><li>Primeiro</li><li>Segundo</li></ol>`           |
| Lista de descrição | `<dl>`, `<dt>`, `<dd>` | `<dl><dt>HTML</dt><dd>Linguagem de marcação</dd></dl>` |

---

## 🧩 6. Tabelas

```html
<table border="1">
    <tr>
        <th>Nome</th>
        <th>Idade</th>
    </tr>
    <tr>
        <td>Pedro</td>
        <td>25</td>
    </tr>
</table>
```

### Explicando:

* `<table>` → tabela
* `<tr>` → linha
* `<th>` → célula de cabeçalho
* `<td>` → célula de dados

---

## 🧍 7. Formulários

```html
<form action="/enviar" method="post">
    <label for="nome">Nome:</label>
    <input type="text" id="nome" name="nome"><br><br>

    <label for="idade">Idade:</label>
    <input type="number" id="idade" name="idade"><br><br>

    <label for="mensagem">Mensagem:</label><br>
    <textarea id="mensagem" name="mensagem"></textarea><br><br>

    <button type="submit">Enviar</button>
</form>
```

| Tag          | Função                                       |
| ------------ | -------------------------------------------- |
| `<form>`     | Cria um formulário                           |
| `<input>`    | Campo de entrada (texto, senha, número etc.) |
| `<textarea>` | Caixa de texto maior                         |
| `<button>`   | Botão                                        |
| `<label>`    | Rótulo de campo                              |

---

## 🎨 8. Estrutura e layout

| Tag         | Função                    | Exemplo                           |
| ----------- | ------------------------- | --------------------------------- |
| `<div>`     | Divisão genérica de bloco | `<div>Conteúdo</div>`             |
| `<span>`    | Trecho em linha           | `<span>Texto colorido</span>`     |
| `<header>`  | Cabeçalho da página       | `<header>Título do site</header>` |
| `<nav>`     | Menu de navegação         | `<nav>Links</nav>`                |
| `<section>` | Seção da página           | `<section>Conteúdo</section>`     |
| `<article>` | Artigo independente       | `<article>Notícia</article>`      |
| `<footer>`  | Rodapé da página          | `<footer>Rodapé</footer>`         |

### Exemplo de layout simples:

```html
<header><h1>Meu Site</h1></header>
<nav><a href="#">Home</a> | <a href="#">Contato</a></nav>
<section>
    <h2>Bem-vindo!</h2>
    <p>Conteúdo principal aqui.</p>
</section>
<footer>&copy; 2025 Meu Site</footer>
```

---

## 🔊 9. Mídia

### Áudio

```html
<audio controls>
  <source src="musica.mp3" type="audio/mpeg">
  Seu navegador não suporta áudio.
</audio>
```

### Vídeo

```html
<video width="320" height="240" controls>
  <source src="video.mp4" type="video/mp4">
  Seu navegador não suporta vídeo.
</video>
```

---

## 💡 10. Comentários

```html
<!-- Isso é um comentário e não aparece na página -->
```

---

## 🔚 Conclusão

O **HTML organiza a estrutura e o conteúdo** de uma página.
Ele é a base da web e é usado junto com:

* **CSS** → para o estilo e aparência.
* **JavaScript** → para interatividade e lógica.

---

## 💻 Exemplo final completo

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Site de Exemplo</title>
</head>
<body>
    <header>
        <h1>Bem-vindo ao Meu Site</h1>
    </header>

    <nav>
        <a href="#">Início</a> |
        <a href="#">Sobre</a> |
        <a href="#">Contato</a>
    </nav>

    <section>
        <h2>Apresentação</h2>
        <p>Este é um exemplo de página HTML com diversas tags em ação!</p>
    </section>

    <footer>
        <p>&copy; 2025 - Desenvolvido para aulas de HTML</p>
    </footer>
</body>
</html>
```

---

## 🧰 Comandos Git úteis

```bash
# Inicia um repositório
git init

# Adiciona todos os arquivos para commit
git add .

# Faz o commit (salva uma versão)
git commit -m "Primeiro commit"

# Conecta ao repositório remoto
git remote add origin git@github.com:usuario/repositorio.git

# Envia os arquivos para o GitHub
git push -u origin master
```

---

📘 **Material didático criado para aulas de introdução à programação – HTML Básico**
👨‍🏫 Professor: *[Pedro Figueiredo]*
📅 Ano: 2025