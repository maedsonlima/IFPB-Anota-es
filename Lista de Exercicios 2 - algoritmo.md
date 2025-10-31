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

```py

```

```py

```

```py

```

```py

```

```py

```

```py

```

```py

```

```py

```

```py

```

```py

```

```py

```

```py

```

```py

```

```py

```

```py

```

```py

```

```py

```

```py

```

```py

```

```py

```

```py

```

```py

```

```py

```
