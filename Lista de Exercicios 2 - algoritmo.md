# - LISTA DE EXERCÍCIOS 1 - 

## 1. Faça um programa que solicite ao usuário dois números e mostre todos os resultados de possíveis de operações relacionais entre eles, ou seja, deve mostrar todos os resultados das operações iniciando com um número e depois com outro. Por exemplo:

○ Usuário informa **6 e 8**

a) Então, por exemplo, o programa deve imprimir os resultados de **6 > 8 e 6 < 8**, e repetindo essa mesma lógica para todas as outras operações relacionais existentes;
b) Os resultados devem ser impressos no seguinte formato: “O valor da avaliação da expressão **6 > 8 é False**”.
```py
num1 = int(input("Insira o 1 número: "))
num2 = int(input("Insira o 2 número: "))

print(f"PELA ÓTICA DO {num1}")
print(f"\nO valor da avaliação da expressão {num1} > {num2} é {num1 > num2} e {num1} < {num2} é {num1 < num2}.")
print(f"O valor da avaliação da expressão {num1} >= {num2} é {num1 >= num2} e {num1} <= {num2} é {num1 <= num2}.")
print(f"O valor da avaliação da expressão {num1} == {num2} é {num1 == num2}.")  
print(f"O valor da avaliação da expressão {num1} != {num2} é {num1 != num2}.") 

print(f"\nPELA ÓTICA DO {num2}")
print(f"O valor da avaliação da expressão {num2} > {num1} é {num2 > num1} e {num2} < {num1} é {num2 < num1}.")
print(f"O valor da avaliação da expressão {num2} >= {num1} é {num2 >= num1} e {num2} <= {num1} é {num2 <= num1}.")
print(f"O valor da avaliação da expressão {num2} == {num1} é {num2 == num1}.")  
print(f"O valor da avaliação da expressão {num2} != {num1} é {num2 != num1}.")   
```
RESULTADO: 

Insira o 1 número: 6
Insira o 1 número: 8
PELA ÓTICA DO 6

O valor da avaliação da expressão 6 > 8 é False e 6 < 8 é True.
O valor da avaliação da expressão 6 >= 8 é False e 6 <= 8 é True.
O valor da avaliação da expressão 6 == 8 é False.
O valor da avaliação da expressão 6 != 8 é True.

PELA ÓTICA DO 8
O valor da avaliação da expressão 8 > 6 é True e 8 < 6 é False.
O valor da avaliação da expressão 8 >= 6 é True e 8 <= 6 é False.
O valor da avaliação da expressão 8 == 6 é False.
O valor da avaliação da expressão 8 != 6 é True.

---
## - 2. Faça um programa que faça o mesmo que o programa anterior, mas agora solicitando Strings ao usuário.
```py
nome1 = input("Insira o 1 nome: ")
nome2 = input("Insira o 2 nome: ")

print(f"PELA ÓTICA DO {nome1}")
print(f"\nO valor da avaliação da expressão {nome1} > {nome2} é {nome1 > nome2} e {nome1} < {nome2} é {nome1 < nome2}.")
print(f"O valor da avaliação da expressão {nome1} >= {nome2} é {nome1 >= nome2} e {nome1} <= {nome2} é {nome1 <= nome2}.")
print(f"O valor da avaliação da expressão {nome1} == {nome2} é {nome1 == nome2}.")  
print(f"O valor da avaliação da expressão {nome1} != {nome2} é {nome1 != nome2}.") 

print(f"\nPELA ÓTICA DO {nome2}")
print(f"O valor da avaliação da expressão {nome2} > {nome1} é {nome2 > nome1} e {nome2} < {nome1} é {nome2 < nome1}.")
print(f"O valor da avaliação da expressão {nome2} >= {nome1} é {nome2 >= nome1} e {nome2} <= {nome1} é {nome2 <= nome1}.")
print(f"O valor da avaliação da expressão {nome2} == {nome1} é {nome2 == nome1}.")  
print(f"O valor da avaliação da expressão {nome2} != {nome1} é {nome2 != nome1}.")   
```
RESULTADO:

PELA ÓTICA DO maedson

O valor da avaliação da expressão maedson > maedson é False e maedson < maedson é False.
O valor da avaliação da expressão maedson >= maedson é True e maedson <= maedson é True.
O valor da avaliação da expressão maedson == maedson é True.
O valor da avaliação da expressão maedson != maedson é False.

PELA ÓTICA DO maedson
O valor da avaliação da expressão maedson > maedson é False e maedson < maedson é False.
O valor da avaliação da expressão maedson >= maedson é True e maedson <= maedson é True.
O valor da avaliação da expressão maedson == maedson é True.
O valor da avaliação da expressão maedson != maedson é False.
---
## - 3. Para vários tributos, a base de cálculo é o salário-mínimo. Faça um algoritmo em Python que leia o valor do salário-mínimo e o valor do salário de uma pessoa. Em seguida, o programa deve calcular e imprimir quantos salários-mínimos a pessoa ganha.

```py
salarioMinimo = float(input("Insira o salário mínimo vigente: "))
salarioReal = float(input("Insira o salário mínimo real: "))

nDeSalarios = salarioReal / salarioMinimo

print(f"O número de salários que você ganha é: {nDeSalarios:.1f} salários mínimos")
```
## 4. Crie um algoritmo em Python que leia o peso de uma pessoa (em kg) e, em seguida, calcule e imprima o peso da pessoa em gramas e o novo peso (também em gramas) se a pessoa aumentar seu peso em 12%.
```py
peso = float(input("Insira seu peso em KG: "))

print(f"seu peso em gramas é: {peso * 1000} Gramas, E seu peso com mais 12% é {((peso * 0.12) + peso) * 1000} Gramas")

```
## - 5. Complete a tabela abaixo com os valores resultantes de avaliação do operador
AND para cada uma das combinações de valores dados:

```py
Valor   1 Valor 2   Resultado do and
False   False
False   True
True    False
True    True
```
False and False = False
False and True  = False
True  and False = false
True  and True  = True

---
## 6. Agora, faça um programa em Python, que mostra o resultado do AND na tela para todas as combinações de valores vistas na questão anterior. A impressão será no formato: “O resultado da operação True and True é “ e o valor da resposta.
```py
valor1 = False
valor2 = False
print(f"O resultado da operação {valor1} and {valor2} é {valor1 and valor2}")

valor1 = False
valor2 = True
print(f"O resultado da operação {valor1} and {valor2} é {valor1 and valor2}")

valor1 = True
valor2 = False
print(f"O resultado da operação {valor1} and {valor2} é {valor1 and valor2}")

valor1 = True
valor2 = True
print(f"O resultado da operação {valor1} and {valor2} é {valor1 and valor2}")
```
---
## 7. Em que ordem a expressão w = x * y < z / x or x / y > z * x and z * y < x seria
avaliada pelo Python? Descreva com detalhes essa ordem, justificando sua
resposta.
```py
Multiplicações e divisões primeiro (* e /)

Depois comparações (< e >)

Depois o and

Por último o or


w = ((x * y < z / x) or ((x / y > z * x) and (z * y < x)))
```
8. Agora, faça um programa que receba os valores de x, y e z do usuário e mostre
o resultado da expressão da questão anterior.

```py
x=1
y=2
z=3

w = x * y < z / x or x / y > z * x and z * y < x

print (w)
```
---
---
## - EXERCÍCIO BEECROWND
Leia 2 valores de ponto flutuante de dupla precisão A e B, que correspondem a 2 notas de um aluno. A seguir, calcule a média do aluno, sabendo que a nota A tem peso 3.5 e a nota B tem peso 7.5 (A soma dos pesos portanto é 11). Assuma que cada nota pode ir de 0 até 10.0, sempre com uma casa decimal.

**Entrada**
O arquivo de entrada contém 2 valores com uma casa decimal cada um.

**Saída**
Imprima a mensagem "MEDIA" e a média do aluno conforme exemplo abaixo, com 5 dígitos após o ponto decimal e com um espaço em branco antes e depois da igualdade. Utilize variáveis de dupla precisão (double) e como todos os problemas, não esqueça de imprimir o fim de linha após o resultado, caso contrário, você receberá "Presentation Error".


Ex de entrada: 
5.0
7.1

ex de saida: 
MEDIA = 6.43182
```py
A = float(input())
B = float(input())

media = (A * 3.5 + B * 7.5) / 11

print(f"MEDIA = {media:.5f}")
```
## - Leia 3 valores, no caso, variáveis A, B e C, que são as três notas de um aluno. A seguir, calcule a média do aluno, sabendo que a nota A tem peso 2, a nota B tem peso 3 e a nota C tem peso 5. Considere que cada nota pode ir de 0 até 10.0, sempre com uma casa decimal.

Entrada
O arquivo de entrada contém 3 valores com uma casa decimal, de dupla precisão (double).

Saída
Imprima a mensagem "MEDIA" e a média do aluno conforme exemplo abaixo, com 1 dígito após o ponto decimal e com um espaço em branco antes e depois da igualdade. Assim como todos os problemas, não esqueça de imprimir o fim de linha após o resultado, caso contrário, você receberá "Presentation Error".

Exemplos de Entrada	Exemplos de Saída
5.0
6.0
7.0

MEDIA = 6.3
```py
A = float(input(""))
B = float(input(""))
C = float(input(""))

media = (A*2 + B*3 + C*5) /10

print(f"MEDIA = {media:.1f}")
```
---
---
### - 12/11/2025 - FOR

Tabuada de 1 a 10 usando for:
```py
for numero in range(1,11): 
    for b in range(1,11):
       print(f"{numero} x {b} = {numero*b}")
```

```py

```

```py

```

```py

```

```py

```

```py

```

```py

```

```py

```

```py

```

```py

```

```py

```

```py

```

```py

```

```py

```

```py

```

```py

```

```py

```
