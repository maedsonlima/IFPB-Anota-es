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

- Muitos inputs estão **sem `name`** → **sem `name`, o valor não é enviado** ao servidor.
- Para upload funcionar, o formulário deve ser:
  ```html
  <form method="POST" action="processaform.html" enctype="multipart/form-data">


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
