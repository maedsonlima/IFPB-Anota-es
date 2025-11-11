### ESCLARECENDO O CÓDIGO INICIAL ABAIXO:
```html
<!DOCTYPE html>
<html>
    <head>
        <title>Portfólio</title>
    </head>
    <body>
        <h1>Isso é um título</h1>
        <p>Isso é um parágrafo</p>
        <img scr="html.png" alt="Logo do HTML 5">
    </body>
</html>
````
```html
<!DOCTYPE html>
````
O !DOCTYPE html declara que será utilizado o HTML5
```html
<html></html>
```
<html> Significa que tudo que estiver entre sua abertura e fechamento será parte do html.
  
```html
<head></head>
````
É a meta informação que fica no canto da pagina, ali na aba  
```html
<title>Portifólio</title>
````
Insere o titulo dentro do canto da página citado acima
```html
<body></body>
````
O Body é propriamente a parte visível do código, onde inserimos titulos, subtitulos, parágrafos, imagens, etc. 
```html
<h1>Isso é um título </1>
````
h1 é o título visível, ele pode ir até h6, quanto maior menor fica o tamanho da letra, podendo ser usado para subtitulo também.
```html
<p>Isso é um parágrafo</p>
````
"P" Insere parágrafos, é importante declarar.

```html
<img src="dali.jpg" alt="A tentação de Santo Antão, Salvador Dali">
````
Aqui é como inserimos imagens, temos algumas observações:

- *<img >* não precisa fechar, ela indica que vamos inserir a imagem no local
- *src=* significa search, é o nome do nosso arquivo (deve estar na mesma pasta do projeto
- *alt* = é apenas uma descrição do que é a imagem, não aparece na página principal.
---
---
## curso 3 - HTML e CSS ambientes de desenvolvimento, estrutura de arquivos e tags
---
---
### aula 3.0 -  CORPO BASE BASE DE UMA PÁGINA 
```html
<!DOCTYPE html>
<html lang="pt-br"a>
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Meu Portifólio</title>
</head>
<body>
    <header></header>
    <main></main>
    <footer></footer>
</body>
</html>
````
### ESCLARECENDO AS NOVAS TAGS:
```html
<html lang="pt-br"> 
````
Lang é a linguagem que ultilizaremos, no caso português Brasil
```html
<meta charset="UTF-8">
````
Dicionário de caracteres que serão ultilizados, deixar esse é o mais usado. Ele engloba todos que ultilizamos inclusive inglês

## OBS: PRIMEIRA COISA QUE DEVEMOS COLOCAR NO CÓDIGO DENTRO DO HEAD, ASSIM:
```
<meta charset="UTF-8">
<html>
    <head>
        <title>Projeto 1 - página</title>
    </head>
    <body>TESTE UM</body>
</html>

```
---
### - HTML 5 - DETALHES IMPORTANTES

```
<!DOCTYPE html>

```
Comentário importante para o navegador saber que é um arquivo HTML - Boas práticas
```
<html lang= "pt-br">
```
É a linguagem de quem está vai ultilizar o site, podemos substituir por outras opções, como:
```
<html lang= "pt-pt">
```
Nesse caso está em portugues de portugal

---
### - INSERINDO PARÁGRAFOS

1- não vamos deixar nada solto no <body>, precisamos ultilizar uma tag, no caso
```html
<p></p>
```
ficando assim:
```html
<!DOCTYPE html>
<html lang= "pt-br"></html>
<html>
    <head>
        <meta charset="UTF-8">
        <title>Projeto 1 - página</title>
    </head>
    <body>
<p>TESTE UM/<p></body>
</html>
```
Agora ele criou um parágrafo
---
### - Inserindo quebra de linha e linhas e cores
```html
<hr color= "green">
```
hr cria a linha, e dentro deles podemos inserir as cores como está acima

---
---
---
## - CÓDIGO DO PROFESSOR ESCLARECIDO
```html
<!DOCTYPE html>
<html>

<head>
<meta charset="utf-8"/>
<title>Meu primeiro formulário</title>
</head>

<body>
<form name="form1" action="processaform.html" method="POST">
<fieldset>
<legend>Login/Senha</legend>
<input type="text" size="50" maxlength="30" placeholder="Nome"/>
<br/>
<input type="password" size="50" maxlength="30" placeholder="senha"/>
</fieldset>
<fieldset>
<legend>Qual país venceu a última olimpíada de programação?</legend>
<input type="radio" value="1" name="conjunto" /><label>Brasil</label>
<br/>
<input type="radio" value="2" name="conjunto" /><label>EUA</label>
<br/>
<input type="radio" value="3" name="conjunto" /><label>Inglaterra</label>
<br/>
<input type="radio" value="4" name="conjunto" /><label>Rússia</label>
</fieldset>
<fieldset>
<legend>Quais países participaram da última copa do mundo?</legend>
<input type="checkbox" value="1" name="grupo" checked/><label>Brasil</label>
<br/>
<input type="checkbox" value="2" name="grupo" /><label>EUA</label>
<br/>
<input type="checkbox" value="3" name="grupo" /><label>Inglaterra</label>
<br/>
<input type="checkbox" value="4" name="grupo" /><label>Rússia</label>
</fieldset>
<fieldset>
<legend>Qual país venceu a última olimpíada de programação?</legend>
<select size="1">
<option>Selecione aqui o país...</option>
<option>Brasil</option>
<option>EUA</option>
<option>Inglaterra</option>
<option>Rússia</option>
</select>
</fieldset>
<label>Selecione uma foto:</label>
<br/>
<input type="file" name="meuarquivo"/>
<hr>
<input type="reset" name="r0" value="LIMPAR"/>
<button type="submit">Ok</button>
<button type="button" onclick="alert('UHULL')">FAZ NADA</button>
<input type="date" />
</form>

<br>
<fieldset>
<legend>DATALIST </legend>
<INPUT TYPE="color" value="#232CAF" name="cor"> <br>
<INPUT TYPE="emai" name="email"> <br>
<INPUT TYPE="month"> <br>
<INPUT TYPE="number" value="10"> <br>
<INPUT TYPE="range" value="70"> <br>
<INPUT TYPE="search"> <br>
<INPUT TYPE="time" value="15:30"> <br>
<INPUT TYPE="url" value="http://"> <br>
<INPUT TYPE="file" name="arquivos"/>
</fieldset>

</body>

</html>
```
# Explicação do Código HTML do Formulário

## Explicação linha a linha

1. `<!DOCTYPE html>` — Declara que o documento usa o padrão HTML5.
2. `<html>` — Elemento raiz que envolve todo o conteúdo HTML.
3. `<head>` — Contém informações internas da página que não são exibidas diretamente.
4. `<meta charset="utf-8"/>` — Define o padrão de caracteres como UTF-8 (evita problemas com acentos).
5. `<title>Meu primeiro formulário</title>` — Define o título exibido na aba do navegador.
6. `</head>` — Finaliza o cabeçalho.
7. `<body>` — Início da parte visível da página.
8. `<form name="form1" action="processaform.html" method="POST">`  
   Criação de um formulário:
   - `action`: página que irá receber os dados.
   - `method="POST"`: envia os dados sem aparecer na URL.
   *(Obs.: Como existe upload de arquivo, deveria ter `enctype="multipart/form-data"` para funcionar corretamente.)*

### Primeiro Fieldset
9. `<fieldset>` — Agrupa elementos relacionados visualmente.
10. `<legend>Login/Senha</legend>` — Título do grupo.
11. `<input type="text" size="50" maxlength="30" placeholder="Nome"/>` — Campo de texto, mas **sem `name`**, por isso **não será enviado**.
12. `<br/>` — Quebra de linha.
13. `<input type="password" size="50" maxlength="30" placeholder="senha"/>` — Campo de senha, também **sem `name`**.
14. `</fieldset>`

### Segundo Fieldset (Botões de seleção - Radio)
15. `<fieldset>`
16. `<legend>Qual país venceu a última olimpíada de programação?</legend>`
17. Cada `<input type="radio" name="conjunto" value="X"/>` representa uma opção exclusiva:
    - Todos compartilham o mesmo `name="conjunto"`, garantindo que apenas um pode ser escolhido.
18. `</fieldset>`

### Terceiro Fieldset (Checkbox)
19. `<fieldset>`
20. `<legend>Quais países participaram da última copa do mundo?</legend>`
21. `<input type="checkbox" name="grupo" value="X"/>` — Permite marcar mais de um item, pois todos usam o mesmo nome.
22. `checked` — Já inicia marcado por padrão.
23. `</fieldset>`

### Quarto Fieldset (Select)
24. `<fieldset>`
25. `<legend>Qual país venceu a última olimpíada de programação?</legend>`
26. `<select size="1">` — Caixa de seleção, mas **sem `name`**, por isso **não enviará valor**.
27. Várias `<option>` formam as opções do menu.
28. `</fieldset>`

### Upload de Arquivo
29. `<label>Selecione uma foto:</label>`
30. `<input type="file" name="meuarquivo"/>` — Permite selecionar um arquivo para envio.  
   *(Repetindo: para funcionar, o `<form>` deve ter `enctype="multipart/form-data"`.)*

### Botões
31. `<input type="reset" value="LIMPAR"/>` — Limpa o formulário.
32. `<button type="submit">Ok</button>` — Envia o formulário.
33. `<button type="button" onclick="alert('UHULL')">FAZ NADA</button>` — Executa um alerta, não envia o formulário.
34. `<input type="date" />` — Campo de data, mas **sem `name`**, portanto **não será enviado**.
35. `</form>` — Final do formulário.

### Fieldset extra (fora do form)
36. `<fieldset>`
37. Diversos `<input>` demonstrando tipos de campos:
   - `type="color"` — Seletor de cores.
   - `type="email"` — Campo com validação de email. *(No código está "emai", o que é erro.)*
   - `type="month"` — Escolha mês e ano.
   - `type="number"` — Apenas números.
   - `type="range"` — Controle deslizante.
   - `type="search"` — Campo de busca.
   - `type="time"` — Seleção de horário.
   - `type="url"` — Validação de URL.
   - `type="file"` — Seleção de arquivo.
38. `</fieldset>`
39. `</body>` — Finaliza conteúdo visível.
40. `</html>` — Finaliza o documento HTML.

---

## Resumo das Tags Utilizadas

| Tag | Função |
|-----|--------|
| `<!DOCTYPE html>` | Indica que o documento segue o padrão HTML5. |
| `<html>` | Contém todo o código da página. |
| `<head>` | Guarda informações internas, como título e configuração. |
| `<meta charset="utf-8">` | Permite o uso de acentos e caracteres especiais. |
| `<title>` | Define o nome exibido na aba do navegador. |
| `<body>` | Tudo que aparece na página ao acessar. |
| `<form>` | Agrupa campos que serão enviados ao servidor. |
| `<fieldset>` | Agrupa visualmente campos relacionados. |
| `<legend>` | Título descritivo do fieldset. |
| `<input>` | Campo de entrada, que muda conforme o atributo `type`. |
| `<label>` | Texto que identifica um campo. |
| `<br>` | Quebra de linha. |
| `<hr>` | Linha horizontal para separação visual. |
| `<select>` | Menu suspenso com opções. |
| `<option>` | Opção dentro do `<select>`. |
| `<button>` | Botão clicável com comportamento definido por `type`. |

---

## Observações Importantes

# 📋 Listas em HTML — Explicação Completa

As **listas em HTML** servem para organizar informações de forma estruturada e visual.  
Elas podem ser:

- 🔢 **Listas ordenadas** (com números, letras ou algarismos romanos)
- ⚫ **Listas não ordenadas** (com marcadores)
- 📖 **Listas de definição** (termos e descrições)

---

## 🔢 Lista Ordenada (`<ol>`)

Uma **lista ordenada** mostra os itens em uma sequência definida, como 1, 2, 3… ou A, B, C…

### 🧩 Como montar:
Use a tag `<ol>` para criar a lista e `<li>` para cada item.

```html
<ol type="a">
  <li>Flamengo</li>
  <li>Vasco</li>
  <li>Corinthians</li>
  <li>São Paulo</li>
  <li>Cruzeiro</li>
</ol>

| Tipo       | Resultado     | Descrição                     |
| ---------- | ------------- | ----------------------------- |
| `type="1"` | 1, 2, 3...    | Números (padrão)              |
| `type="a"` | a, b, c...    | Letras minúsculas             |
| `type="A"` | A, B, C...    | Letras maiúsculas             |
| `type="i"` | i, ii, iii... | Algarismos romanos minúsculos |
| `type="I"` | I, II, III... | Algarismos romanos maiúsculos |

```
⚫ Lista Não Ordenada (<ul>)

Uma lista não ordenada mostra os itens com marcadores, em vez de números.

🧩 Como montar:

Use a tag <ul> para iniciar a lista e <li> para cada item.
```html
<ul type="disc">
  <li>Flamengo</li>
  <li>Vasco</li>
  <li>Corinthians</li>
  <li>São Paulo</li>
  <li>Cruzeiro</li>
</ul>

```
| Tipo            | Resultado | Descrição           |
| --------------- | --------- | ------------------- |
| `type="disc"`   | ●         | Padrão (bola cheia) |
| `type="circle"` | ○         | Círculo vazio       |
| `type="square"` | ■         | Quadrado            |
| `type="none"`   | —         | Nenhum marcador     |


📖 Lista de Definição (<dl>)

As listas de definição servem para criar termos seguidos de suas explicações — como se fosse um glossário.

🧩 Como montar:

Use <dl> para iniciar a lista, <dt> para o termo, e <dd> para a descrição.
```html
<dl>
  <dt>Título 1</dt>
  <dd>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</dd>

  <dt>Título 2</dt>
  <dd>Beatae architecto, doloremque, quisquam.</dd>

  <dt>Título 3</dt>
  <dd>Consectetur adipisicing elit. Beatae, architecto!</dd>
</dl>

```
🧱 Estrutura:

<dl> → inicia a lista de definição

<dt> → define o termo (título)

<dd> → define a descrição do termo


🌐 Listas Aninhadas (Listas dentro de outras)

Você pode colocar uma lista dentro de outra, criando subníveis de organização.

🧩 Exemplo:
```html
<ul type="disc">
  <li>
    São Paulo
    <ol type="1">
      <li>Santo André</li>
      <li>São Bernardo</li>
      <li>São Caetano</li>
    </ol>
  </li>
</ul>

<ul type="disc">
  <li>
    Paraíba
    <ol type="1">
      <li>Lagoa Seca</li>
      <li>Lagoa de Dentro</li>
      <li>Lagoa de Roça</li>
    </ol>
  </li>
</ul>




``````html

```
👉 Dica:
A lista interna pode ser <ol> (ordenada) ou <ul> (não ordenada).
Você pode misturar tipos conforme quiser.

---
🧱 Tabelas em HTML

Tabelas organizam informações em linhas e colunas, ideais para dados estruturados.

🧩 Exemplo:
```html
<table border>
  <tr>
    <td colspan="3">L1 C1</td>
  </tr>
  <tr width="100%">
    <td width="20%">L2 C1</td>
    <td width="60%">L2 C2</td>
    <td width="20%">L2 C3</td>
  </tr>
  <tr width="100%">
    <td width="20%">L3 C1</td>
    <td width="60%">L3 C2</td>
    <td width="20%">L3 C3</td>
  </tr>
  <tr width="100%">
    <td width="20%">L4 C1</td>
    <td width="60%">L4 C2</td>
    <td rowspan="2">L4 C3</td>
  </tr>
</table>

```
🏷️ Resumo das Tags Usadas
Tag	Função
<ol>	Cria lista ordenada
<ul>	Cria lista não ordenada
<li>	Cria um item da lista
<dl>	Cria uma lista de definição
<dt>	Define o termo da lista de definição
<dd>	Define a descrição do termo
<table>	Cria uma tabela
<tr>	Cria uma linha da tabela
<td>	Cria uma célula da tabela
colspan	Mescla colunas
rowspan	Mescla linhas
<br>	Quebra de linha
<hr>	Linha divisória horizontal
<p>	Define um parágrafo



---
---
CÓDIGO PRONTO
``````html
<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<title>Prova de HTML</title>
<style>
    body {
        background-color: #D3D3D3;
        font-family: Arial, sans-serif;
    }
    table {
        width: 100%;
        border: 1px solid black;
        border-collapse: collapse;
    }
    th, td {
        border: 1px solid black;
        padding: 5px;
    }
    .menu {
        text-align: center;
        font-weight: bold;
        background-color: #E0E0E0;
    }
    .menu a {
        margin: 0 20px;
        text-decoration: none;
        color: blue;
        font-weight: bold;
    }
    .titulo {
        font-weight: bold;
        font-size: 24px;
    }
    .subtitulo {
        font-weight: bold;
        font-style: italic;
    }
    .form-tabela td:first-child {
        width: 30%;
    }
    .form-tabela td:last-child {
        width: 70%;
    }
    input[type="text"], input[type="password"], textarea {
        width: 95%;
    }
    input[type="button"], input[type="submit"] {
        margin: 5px;
    }
</style>
</head>
<body>

<!-- MENU -->
<table>
    <tr class="menu">
        <td rowspan="2" width="10%">
            <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/42/Thumbs_up_icon.svg/768px-Thumbs_up_icon.svg.png" width="70">
        </td>
        <td colspan="4">MENU DA PROVA</td>
    </tr>
    <tr class="menu">
        <td><a href="#">HOME</a></td>
        <td><a href="#">CONTEUDO1</a></td>
        <td><a href="#">CONTEUDO2</a></td>
        <td><a href="#">CONTATO</a></td>
    </tr>
    <tr>
        <td colspan="5" align="center"><b>PROVA DE HTML</b></td>
    </tr>
</table>

<!-- CONTEÚDO -->
<h2 class="titulo">Titulo1</h2>
<p><span class="subtitulo">Esse texto esta em negrito e em italico</span></p>

<ul>
    <li><b><u>Tarefas do dia de hoje</u></b>
        <ol>
            <li>trabalhar</li>
            <li>estudar</li>
            <li>fazer a prova</li>
        </ol>
    </li>
    <li><b><u>Tarefas do dia de amanha</u></b>
        <ol>
            <li>dormir</li>
            <li>acordar</li>
            <li>dormir de novo</li>
        </ol>
    </li>
</ul>

<h2 class="titulo">Titulo2</h2>

<!-- FORMULÁRIO -->
<table class="form-tabela">
    <tr>
        <th colspan="2">FORM DA PROVA</th>
    </tr>
    <tr>
        <td>NOME:</td>
        <td><input type="text" name="nome"></td>
    </tr>
    <tr>
        <td>LOGIN:</td>
        <td><input type="text" name="login"></td>
    </tr>
    <tr>
        <td>SENHA:</td>
        <td><input type="password" name="senha"></td>
    </tr>
    <tr>
        <td>GENERO:</td>
        <td>
            <input type="radio" name="genero" value="masculino"> MASCULINO
            <input type="radio" name="genero" value="feminino"> FEMININO
        </td>
    </tr>
    <tr>
        <td>HOBBY:</td>
        <td>
            <input type="checkbox" name="hobby" value="esportes"> ESPORTES
            <input type="checkbox" name="hobby" value="musica"> MUSICA
            <input type="checkbox" name="hobby" value="cinema"> CINEMA
            <input type="checkbox" name="hobby" value="praia"> PRAIA
        </td>
    </tr>
    <tr>
        <td>NOME:</td>
        <td><textarea rows="3" placeholder="comente aqui...."></textarea></td>
    </tr>
    <tr>
        <td colspan="2" align="center">
            <input type="reset" value="Limpar">
            <input

```

```html

```

``````html

```

```html

```

``````html

```

```html

```

``````html

```

```html

```

``````html

```

```html

```

``````html

```
