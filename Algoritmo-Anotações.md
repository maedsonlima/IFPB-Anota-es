# - Aula 2 - Python - tipos de variáveis

### - Números
- Inteiros, ex: 1
- ponto flutuante, ex: 3.5

### - Strings

Conjunto de caracteres, ex: "Abca#84739"

### - Boleanos

True or False, armazena uma informação binária

ex: de código
```py
nome = "Maedson"
print (nome)

num_pi = 3.14
print(num_pi)
```
Atribuimos  o nome maedson na variável nome e mostranos na tela com o print

---
### - Como descobrir o tipo de variável

ex:
```py
print(type("maedson"))
print(type(8))

```
Ele vai retornar o resultado com o tipo de variável, sendo esse o resultado:
```py
<class 'str'>
<class 'int'>
```
Outro Exemplo com variável
```py
nome = "maedson"
idade = 29
preco = 15.99
aposentado = True
print(type(nome))
print(type(idade))
print (type(preco))
print (type(aposentado))

```
Temos como resultado:
```py
<class 'str'>
<class 'int'>
<class 'float'>
<class 'bool'>
```
Ou seja, ele diz que a classe nome é "string
idade é int = inteiro
e o preco é float, ou seja flutuante
o aposentado é 'bool', ou seja boleeano
---

## -  EXERCÍCIO EXEMPLIFICATIVO- Quais tipos?

1- RECEBA O CÓDIGO DA PEÇA
2- RECEBA O VALOR DA PEÇA
3- RECEBA Q QUANTIDADE DE PEÇAS
4- CALCULE O VALOR TOTAL DA PEÇA (QUANTIDADE * VALOR DA PEÇA)
5- MOSTRE O CÓDIGO DA PELA E SEU VALOR TOTAL

---
---
# - ENTRADA e SAÍDA DE DADOS

```py
input
```
Permite ler informações via teclado do usuário.

## TUDO QUE ELE LER É STRING

Pode ser convertido para (int) ou real (float)

ex:
```py
var = input (String mensagem)
```
var = cria uma variável
input = armazena na variável o que ele ler
( )  dentro dos parenteses insira a mensagem que o usuário vai ler, ex: pedido para inserir informações

ex:
```py
nome = input(" digite seu nome: ") 
```
Para imprimir o nome que o usuário digitou, fazemos:
```py
print(f"o nome digitado é: {nome}")
```
obs: colocamos o f antes das aspas, e lá dentro usamos chaves

Código completo: 
```py
nome = input("insira seu nome: ")
print(f"o nome digitado é: {nome}")
```
---
## - CAST - conversão de String do input para outros tipos

Explicitamos o tipo que queremos guardar, se for número por exemplo usamos:

int = inteiro
floar = flutuante, valores quebrados
etc..

ex:
```py
idade = int(input("Digite sua idade é: "))
print (f"sua idade é {idade})
```
traduzindo: Tudo que for digitado dentro do input, será transformado em INT, e depois será guardado na variável idade. 

RESPEITANDO A REGRA DOS PARENTESES, o que estiver na parte de dentro será realizado primeiro.
---
## - 26/09/25 - AULA  4- CRIANDO VARIÁVEIS PARA CALCULAR NÚMEROS

1- Criamos 2 variáveis

```py
numero1 = int(input("Digite um número inteirp: "))
numero2 = int(input("Digite o segundo número inteiro: "))
```
Ele vai pedir o 1 numero, o usuário insere,
Vai pedir o segundo número, o usuário insere.

### - Somando os números
```py
numero1 = int(input("Digite um número inteirp: "))
numero2 = int(input("Digite o segundo número inteiro: "))
resultado = numero1 + numero2

print (f"o resultado é:  {resultado}")

```
A variável resultado armazena a soma
o print mostra o resultado na tela

ou podemos fazer de forma mais rápida.

```py
print (f"a soma é:  {numero1 + numero2}")

## - DObrando o número

numero = int(input("Digite um número inteiro: "))
dobro = numero * 2 
print (f"o dobro do {numero} é: {dobro}")
```
---
aqui dobramos o número usando o sinal de *, ele multiplica.

---
## - 3 FORMAS DE FAZER PORGENTAGEM DE UM NÚMERO:
```py
salarioInicial = float(input("Digite o salário inicial: "))
porcentagem = (salarioInicial * 20)/100
salarioFInal = porcentagem + salarioInicial
print (f"o {salarioInicial} com 20% é: {salarioFInal}")

salarioInicial = float(input("Digite o salário inicial: "))
porcentagem = (salarioInicial * 20)/100
print (f"o {salarioInicial} com 20% é: {salarioInicial + porcentagem}")


salarioInicial = float(input("Digite o salário inicial: "))
print (f"o {salarioInicial} com 20% é: {salarioInicial * 1.2}")

```
### 1- modo

Explicação

salarioInicial = float(input(...)):
Solicita ao usuário que digite o salário inicial e converte para float (número com casas decimais).

porcentagem = (salarioInicial * 20) / 100:
Calcula 20% do salário.

salarioFInal = porcentagem + salarioInicial:
Soma os 20% ao salário original para obter o salário final.

print(...):
Exibe o valor original e o novo salário com o aumento.

🟡 Observação

A variável salarioFInal está com "F" maiúsculo, o que não segue a convenção usual de nomes em Python (snake_case).

Poderia ser mais direto.


### 2 - MODO

✅ Explicação

Calcula os 20% como no código anterior.

Em vez de guardar o salário final em uma variável, ele soma diretamente dentro do print().

✅ Vantagem

Menos linhas de código (mais direto).

Funcionalmente idêntico ao primeiro

### 3- MODO

✅ Explicação

Cálculo mais eficiente: multiplica o salário por 1.2, que é o mesmo que somar 20%.

Exemplo: 1000 * 1.2 = 1200.

Elimina a necessidade de variáveis intermediárias.

✅ Vantagem

Mais limpo, direto e performático.

Boa prática para casos simples como esse.

---
## - POTÊNCIA DE UM NUMERO SOBRE OUTRO
```py
numero1 = int(input("Digite o primeiro numero: "))
numero2 = int(input("Digite o segundo numero: "))
print (f"O {numero2} elevado ao {numero2} é:{numero1 ** numero2}")
```

recebe os 2 números, e depois coloca o 2 como a potência do 1
---
## - Média aritimédica  de notas
```py
numero1 = float(input("Digite a primeira: "))
numero2 = float(input("Digite a segunda nota: "))
numero3 = float(input("Digite a terceira nota: "))
print (f"a média é:{(numero1 + numero2 + numero3)/3}")
```
Ele vai receber 3 valores, depois vai somar, e dividir por 3.

---
## - VALOR PARCELADO EM 10X
```py
ValorInicial= float(input("Digite o Valor inicial: "))
print (f"{ValorInicial} parcelado em 10x é : 10x de: {ValorInicial/10}")
```
---
# - LISTA DE EXERCÍCIOS 1 - 

1. Faça um programa que peça um número natural ao usuário e imprima o quadrado desse número.
```py
numero = int(input("Insira o número: "))
print (f"Seu número ao quadrado é {numero*numero}")

```

2. Faça um programa que peça dois números naturais ao usuário e imprima a divisão do primeiro número pelo segundo. Avise ao usuário que o segundo número não pode ser 0.
```py
print ("Bem vindo a cálculadora de divisão")
numero1 = int(input("Insira o número que será dividido: "))
numero2 = int(input("Insira o divisor. obs: diferente de 0): "))
print (f"{numero1} divido por {numero2} é {numero1/numero2}")

```

3. Escreva um programa que peça ao usuário um número natural que representa o lado de um quadrado e calcule seu perímetro e a sua área.
```py
print ("Cálculadora de área/perimetro de um Quadrado.")
lado = int(input("Insira o tamanho do lado do quadrado: "))
perimetro = (lado * 4)
area = (lado * lado)
print (f"O quadrado cujo lado é {lado}, tem como área {area} e perimetro {perimetro}")

```
4. Escreva um programa que peça ao usuário dois números naturais para as variáveis A e B, e efetue as trocas dos valores de forma que a variável A passe a possuir o valor da variável B e a variável B passe a possuir o valor da variável A. Apresentar os valores trocados. OBS: não é permitido apenas imprimir o valor trocado. Ex.: “O valor da variável A é: “ e imprimir da variável B.
```py
variavelA = int(input("Iinsira a variável A: "))
variavelB = int(input("Iinsira a variável B: "))
caixaDeTroca = variavelA
variavelA = variavelB
variavelB = caixaDeTroca
print (f" A variavel A é :{variavelA}, A variável B é: {variavelB}")

```
5. Escreva um programa que efetue a apresentação do valor da conversão em real (R$) de um valor lido em dólar (US$). O algoritmo deverá solicitar ao usuário o valor da cotação do dólar, e também a quantidade de dólares que ele deseja converter.
```py
print ("Bem vindo o conversor de USD para BRL")
cotacao = float(input("Insira o valor da cotação de USD atual: "))
valorEmDolar = float(input("Insira o valor que deseja converter: "))
print (f"{valorEmDolar} em reais BRL é: {cotacao * valorEmDolar}")

```
6. Escreva um programa que leia uma temperatura em graus Celsius e a apresente convertida em graus Fahrenheit. A fórmula de conversão é: F = (9*C+160) / 5, sendo F a temperatura em Fahrenheit, e C a temperatura em Celsius.
```py
print ("Bem vindo o conversor de Celcius para Fahrenheit")
celcius = float(input("Insira a temperatura em Celcius: "))
fahrenheit = (9*celcius + 160)/5    
print (f"{celcius} Celcius convertidos em Fahrenheit é: {fahrenheit}")

```
7. Uma empresa quer dar um bônus de Natal (em dezembro, claro) para seus empregados que será 60% do cálculo médio do salário de trabalho. Considerando que todos na empresa ganhem um mesmo valor de salário, elabore um programa que receba a entrada do salário e imprima o valor do bônus de Natal e o valor a ser depositado na conta de cada empregado em dezembro.
```py
print ("Bem vindo a calculadora do Bonus salárial de natal")
salarioBase = float(input("Insira o seu salário: "))
bonus = salarioBase * 0.6  #calcula 60% do salário.    
salarioFinal = salarioBase + bônus

print (f"Seu BONUS de 60% é de: {bonus}")
print (f"O valor final a ser depositado é: {salarioFinal}")

```
8. Crie um algoritmo que efetue o cálculo do salário líquido de um professor. Os dados fornecidos serão: valor da hora aula, número de aulas dadas no mês e percentual de desconto do INSS.
```py
print ("Descubra o seu salário líquido")
horasAula = float(input("Insira o valor das suas horas/aula: "))
quantidadeAulas = int(input("Insira o número de aulas dadas no mês: "))  
percentualInss = float(input("Insira o percentual de desconto do INSS (SEM O %): "))  

salarioBruto = horasAula * quantidadeAulas                      # Calcula o salário sem o desconto
descontoInss = (percentualInss * salarioBruto) / 100     # Calcula a porcentagem descontada em Reais
salarioLiquido = salarioBruto - descontoInss                     # Retira o desconto em Reais do salário Liquido

print (f"Seu salário líquido é de: {salarioLiquido} ")

```

9 - Antes do racionamento de energia ser decretado, quase ninguém falava em quilowatts; mas, agora, todos incorporaram essa palavra em seu vocabulário. Sabendo-se que 100 quilowatts de energia custa um sétimo do salário mínimo, faça um algoritmo que receba o valor do salário mínimo e a quantidade de quilowatts gasta por uma residência, e calcule (imprima):

o  valor em reais de cada quilowatt;
o valor em reais a ser pago;
o novo valor a ser pago por essa residência com um desconto de 10%.

```py
print ("Calcule a energia gasta na sua residência")
salario = float(input("Insira o seu salário: "))
quilowattsGasta = int(input("Insira a quantidade de quilowatts gastas no mês: "))  

valorQuilowatt = (salario/7) / 100                                            #salario /  por 7 = 1/7 de salário, vezes 100 QW
valorTotal = valorQuilowatt * quilowattsGasta                  # O Valor da unidade de QW vezes a quantidade
valorTotalComDesconto = valorTotal * 0.9                          # multiplica por 0.9 porque é 90%, se fosse 100% seria 1.0, retiamos 0.1 = 90%

print (f" O valor de cada Quilowatt é: R${valorQuilowatt:.2f}")
print (f" O valor total é de: R${valorTotal:.2f}")
print (f" O valor total com desconto é de: R${valorTotalComDesconto:.2f}")

```
## - 01/10/2025 AULA 5 -  Formatação de Strings

OBS: Material está no classrom

### Combinando Strings

1- alternativa: usando f-strings : ("f  {} ")
  ex:  ("f  {} ")
```py
idade = 36
mensagem = f"Eu tenho {idade} anos de idade."
print (mensagem)
```
A variávem mensagem vai armazenar o valor da idade também pois ela está linkada com a variável idade

EX 2:
```py
mensagem = f"o produto custa {2*6} reais"
print (mensagem)
```
Aqui a variável "mensagem" armazena o cálculo ( a máquina fará um calculo ali, não é como simplesmente entregar o um caractere representando o número)

ex3: 
```py
print (f"o produto custa {2*6} reais")
```
Nesse caso não é armazenado em nenhuma variável, apenas realiza o cálculo e mostra.

---

## - Formatando valores

Basta adicionar dois pontos seguidos por um tipo de formatação como .2f, que siginifica que o número deve ser tratado como um float com duas casas decimais. 

ex:
```py
preco = 61
print (f"o produto custa {preco:.2f} reais")
 ```
vai imprimir o número 61.00

ex2:
```py
preco = 31.946
print (f"o produto custa {preco:.2f} reais")
```
Vai imprimir 31.95

ex3:
```py
preco = 31.9412
print (f"o produto custa {preco:.2f} reais")
```
imprime 31.94

OBS: Quando pedimos para diminuir as casas decimais, ele vai ARREDONDAR para o valor mais adequado

ex: 

31.946 = ficará 31.95
31.945 = ficará 31.94

---
## - Caracteres de escape

Serve para imprimir caracteres não permitidos em uma string

usamos uma barra invertida para possibilitar: \ 

ex:
```py
texto = "Tenho "sorte" na vida"
```
note que "sorte" tem aspas dentro de outras aspas e não pode, não  imprimiria elas, então usamos a \
```py
texto ="Tenho \"sorte\" na vida"
print (texto)
```
Dessa forma ele vai desconsiderar as aspas para algum fim de programação e vai  imprimir o texto completo.

OBS: a primeira barra e segunda barras são antes das 1 e 2 aspas respectivamente.

SEMPRE QUE QUISER USAR UM SIMBOLO QUE NÃO PODERIA, USE \ ANTES DELE.

---
## - OUTRAS FORMATAÇÕES PARA O TEXTO:

\t = faz uma tabulação no texto, onde quiser, pode usar várias vezes inclusive
\n = pula uma linha.
\\ = imprime uma barra invertida.

```py
textoSemTabuacao = "texto sem tabulação"
textoComTabuacao = "\t texto sem tabulação"

```
Vai imprimir 

texto sem tabulação
         texto sem tabulação
         
A tabulação vai gerar um espaço no início.


### - /n = pulando linha
```py
print ("\nLinha 1 \nLinha 2 \nLinha 3")
```
Saida:

Linha 1 
Linha 2 
Linha 3

Ele vai pular uma linha naquela palavra em específico.

---
### - Imprimindo uma \ invertida, é muito útil para informar caminhos de pastas no computador

ex: 
print ("O arquivo está na pasta: C:\\usuario\\documentos")
```py
print ("O arquivo está na pasta: C:\\usuario\\documentos")
```
Nesse caso colocamos 2 barras, para poder mostrar uma, pois se colocarmos só 1, ele não vai mostrar nada, pois a barra já é usada para transformar simbolos em caracteres, então usando outra, podemos escrever o caminho da pasta sem problemas, ou até meesmo uma barra \\ da forma que quiser.

---
---
## - OPERADORES ARITMÉTICOS


- Adição                        +

- Subtração                     -

- Multiplicação                 *

- Exponenciação                 **

- Divisão                       /

- Parte inteira da Divisão     //

- Resto da divisão             %

ex:
```py
print(4+5*2)

print((4+5)*2)

print(3*3)

print(3**3)

print(10/3)

print(10//3)

print(10%3)
```
Temos como resultado:
18
9
27
3.3333333333333335
3
1
---
## - Operadores Relacionais

Serve para comparar Strings, números, são eles: 

Maior          >
Maior igual    >=
Menor          <
Menor igual    <=
Igualdade      ==
Diferente      !=

Seu resultado é sempre um valor 'BOOLEANO'

EX:
```py
print(10 > 5)
print(256 < 257)
print(997 <= 998)
print(22 != 23)
print(37 == 38)
print('Maria' == 'Pedro’)
print(‘Maria’ == ‘maria’)
print(‘Pedro' == 'Pedro’)
```
Temos como resultado:

True =  10 é maior que 5
True =  256 é menor que 257
True = 997 é menor ou igul a 998
True = 22 é diferente de 23
False = 37 não é igual a 38
False  = maria  não é igual a Pedro
False = Maria não é igual a maria (Case sensitive)
True =  Pedro é igual a Pedro

---
## OPERADORES LÓGICOS 

Servem para combinar resultados de expressões, retornando se
o resultado final é verdadeiro ou falso.

Operação booleana E 'AND'
Operação booleana OU 'OR'
Operação booleana de negação 'NOT'

EX: 
```py
2 < 9 and 4 == 5 and 6 > 1

```
Resolução
2 é menor que 9 = Verdadeiro
4 é diferente de 5 = false
6 é maior que 1  = verdadeiro

como a proposição é AND, logo resultado é FALSO!
---
## - 08/10/2025 -  Continuação - Proposições lógicas.
```py
print (6 + 5 == 11 and 5+5 == 10)
print (5*3 == 15 or not(-30/2==15))

print(not ("laranja" == "estojo"))

```
Exemplo básicos da aula, retorno:

True
True
True
----
### - Abreviação de atribuição:

```py
#x = 10
#x = x + 15

x=10
x+=5
print(x)

```
A operações são iguais

x+=  QUER DIZER QUE É ELE MESMO + ALGUMA COISA QUE VOCÊ ESCOLHER

Serve para outras operações.

x+=
x-=
x*=
x/=  é o proprio numero do x divido por algum numero dps do =
**=
%=
//=

ex:
```py
x= 10
x/= 2
print(x)

```
Resultado = 2.
---
---
## - EXERCÍCIO - 

01. Faça um programa em Python que leia dois números inteiros (A e B), realize
os seguintes cálculos e exiba o resultado de cada cálculo.
a) A parte inteira da divisão entre os valores de A e B
b) O resto da divisão entre os valores de A e B
c) O correspondente a 35 % do valor de B

```py
a = int(input("Insira o primeiro número: "))
b = int(input("Insira o segundo número: "))

print (f"\nAparte inteira de {a} dividido por {b} é {a//b} ")
print (f"\no resto de {a} dividido por {b} é {a%b}")
print (f"\n35% do valor de {b} é {b*0.35}")

```
## - 02. Faça um programa em Python que calcule o total de uma compra e a
comissão do vendedor. Leia a matrícula do vendedor, considere uma compra
com 3 produtos (para cada produto leia a quantidade e o valor por unidade) e
uma comissão de 12% do valor total da compra. No final informe a matrícula do
vendedor, o total da compra e a comissão do vendedor.
```py
matricula = int(input("Insira sua matricula: "))

item1 = int(input("Insira a quantidade do item 1: ")) 
unidade1 = float(input("Insira o valor do item 1: ")) 

item2 = int(input("Insira a quantidade do item 2: ")) 
unidade2 = float(input("Insira o valor do item 2: ")) 

item3 = int(input("Insira a quantidade do item 3: ")) 
unidade3 = float(input("Insira o valor do item 3: ")) 

totalCompra = (item1*unidade1) + (item2*unidade2) + (item3+unidade3)

comissao = totalCompra * 0.12

print (f"\nsua matricula é {matricula} ")
print (f"o total da compra {totalCompra}, sua comissão é {comissao} ")
```
---
### 10/10/2025 - COMANDOS CONDICIONAIS





```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
```py

```

```py

```

```py

```
