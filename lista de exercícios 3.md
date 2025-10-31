## 1- Faça um programa em python que peça um valor e mostre na tela se o valor é positivo ou negativo.

```py
valor = int(input("Insira o valor para verificar: "))

if(valor >= 0):
 print("o número é positivo")
else:
 print("numero negativo")
```
## - 2) Escreva um programa que leia um número e imprima se este número é ímpar ou par.
```py
valor = int(input("Insira o valor para verificar: "))

if(valor%2==0):
 print("o número é par")
else:
 print("numero impar")
```
## 3) Faça um programa que verifique se uma letra digitada é “C”, “S” ou “D”. Conforme a letra, escrever: C - Casado, S - Solteiro, D - Divorciado, Estado Civil Inválido (para qualquer outra letra digitada). 

OBS: Considere que o usuário pode digitar as letras em formato minúsculo.
```py
letra = input("Insira a letra para verificar: ")

if(letra=="C" or letra=="c"):
    print("Casado")
elif(letra =="S" or letra=="s"):
    print("divorciado")
elif(letra =="D" or letra=="d"):
    print("divorciado")
else:
    print("letra inválida")
```
## 4- 4) Faça um programa em python que solicite ao usuário três números e imprima- os em ordem decrescente (do maior para o menor).
```py
numero1 = int(input("Insira o primeiro número: "))
numero2 = int(input("Insira o segundo número: "))
numero3 = int(input("Insira o terceiro número: "))

if (numero1 > numero2 > numero3):
    print(f"{numero1}, {numero2},{numero3}")

elif (numero1 > numero3 > numero2):
    print(f"{numero1},{numero3},{numero2}")

elif (numero2 >numero1 > numero2):
    print(f"{numero2},{numero1},{numero3}")

elif (numero2 >numero3 > numero1):
    print(f"{numero2},{numero3},{numero2}")
    
elif(numero2 >numero1 > numero2):
    print(f"{numero2},{numero1},{numero3}")

elif(numero3 >numero1 > numero2):
    print(f"{numero3},{numero1},{numero2}")
    
else:
     print(f"{numero3},{numero2},{numero1}")

```
## - 5 Faça um programa que verifique se uma letra digitada é vogal ou consoante.
```py
letra = input("digite a letra para verificar: ")

if(letra =="A" or letra =="a"):       
    print("vogal")
elif(letra =="E" or letra =="e"):   
    print("vogal")
elif(letra == "I" or letra =="i"):  
   print("vogal") 
elif(letra =="O" or letra =="o"):   
    print("vogal")
elif(letra =="U" or letra =="u"):   
    print("vogal")
else: 
   print("consoante") 
```
# 6- Faça um programa que leia 3 valores e escreva o produto dos 2 maiores.
```py
a = float(input("Digite o primeiro valor: "))
b = float(input("Digite o segundo valor: "))
c = float(input("Digite o terceiro valor: "))

if a <= b and a <= c:
    print(f"O produto dos dois maiores valores é: {b * c}")
elif b <= a and b <= c:
    print(f"O produto dos dois maiores valores é: {a * c}")
else:
    print(f"O produto dos dois maiores valores é: {a * b}")
```
## 7 - Faça um programa que leia 3 números e calcule a média ponderada entre eles.
Considere que o maior número recebe peso 5 e os outros dois recebem peso
2,5.
```py

if a >= b and a >= c:
    print(f"A média ponderada é: {(a * 5 + b * 2.5 + c * 2.5) / 10}")
elif b >= a and b >= c:
    print(f"A média ponderada é: {(b * 5 + a * 2.5 + c * 2.5) / 10}")
else:
    print(f"A média ponderada é: {(c * 5 + a * 2.5 + b * 2.5) / 10}")
```
## - 8 Faça um programa que pergunte em que turno você estuda. Peça para digitar M (matutino), V (vespertino) ou N (noturno). Imprima a mensagem “Bom Dia!”,  “Boa Tarde!” ou “Boa Noite!” ou “Valor Inválido!”, conforme o caso. OBS: Considere que o usuário pode digitar as letras em formato minúsculo.
```py
turno = input("Em que turno você estuda? (M/V/N): ")

if turno == "m" or turno == "M":
    print("Bom Dia!")
elif turno == "v" or turno == "V":
    print("Boa Tarde!")
elif turno == "n" or turno == "n":
    print("Boa Noite!")
else:
    print("Valor Inválido!")
```
## - 10 Faça um programa que lê nome, estado civil e idade de uma pessoa. Se a pessoa for casada e tiver menos de 25 anos, imprimir nome e a mensagem: ACEITA. Caso contrário, imprimir o nome e a mensagem: NÃO ACEITA. (Para o estado civil casado, o usuário deverá informar C ou c; para o estado civil

solteiro, o usuário deverá informar S ou s; para o estado civil divorciado, o
usuário deverá informar D ou d.)
```py
nome = input("Digite seu nome: ")
estado_civil = input("Digite seu estado civil (C - casado, S - solteiro, D - divorciado): ")
idade = int(input("Digite sua idade: "))

if (estado_civil == "C" or estado_civil == "c") and idade < 25:
    print(f"{nome} - ACEITA")
else:
    print(f"{nome} - NÃO ACEITA")
```
## 11 Uma prefeitura abriu uma linha de crédito para os funcionários estatutários. O valor máximo da prestação não poderá ultrapassar 30% do salário bruto. Faça um algoritmo que solicite ao funcionário informar o seu salário bruto e o valor da prestação, e informe se o empréstimo pode ou não ser concedido para ele.
```py
salario = float(input("Digite o seu salário bruto: "))
prestacao = float(input("Digite o valor da prestação: "))

# Calcula 30% do salário
limite = salario * 0.3

if prestacao <= limite:
    print("Empréstimo pode ser concedido.")
else:
    print("Empréstimo não pode ser concedido.")
```

<img width="645" height="453" alt="image" src="https://github.com/user-attachments/assets/ac460a27-fcca-47c1-b549-38fb1ca68882" />

```py
idade = int(input("Digite sua idade: "))

plano = input("Escolha o plano (E - Enfermaria, A - Apartamento): ")
odontologico = input("Deseja incluir plano odontológico? (S - Sim, N - Não): ")

# Inicializa o valor
valor = 0

# Define o valor base pelo plano de saúde e idade
if idade <= 18:
    if plano == "E" or plano == "e":
        valor = 400
    elif plano == "A" or plano == "a":
        valor = 490
elif 19 <= idade <= 39:
    if plano == "E" or plano == "e":
        valor = 520
    elif plano == "A" or plano == "a":
        valor = 610
elif 40 <= idade <= 59:
    if plano == "E" or plano == "e":
        valor = 640
    elif plano == "A" or plano == "a":
        valor = 740
else:  # 60 anos ou mais
    if plano == "E" or plano == "e":
        valor = 760
    elif plano == "A" or plano == "a":
        valor = 890

# Acrescenta plano odontológico, se desejado
if odontologico == "S" or odontologico == "s":
    valor += 30

print(f"O valor a ser pago pelo plano de saúde é: R${valor}")

```

```py

```

