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

```py

```

```py

```

```py

```

```py

```

```py

```

```py

```

```py

```

