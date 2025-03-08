import random
import time
from datetime import datetime

Distmotorista = random.uniform(1, 5)

print("Ola, seja bem vindo ao Uber")

print()

while True:
    try:
        Distancia = float(input("Qual a distancia que deseja percorrer?(Em km): "))
        break
    except ValueError:
        print("Erro! Por favor, digite um número válido.")

print()

opção = input("UberBlack ou UberX(B ou X): ").strip().lower()
if opção == "b":
   valor = Distancia * random.uniform(2.5, 3)
else:
   valor = Distancia * random.uniform(1.5, 2)

horario = datetime.now().strftime("%H:%M")

if horario < "12:00":
    valor -= 5
elif horario < "18:00":
    valor += 5
else:
    valor += 10

tempo = Distmotorista * 1.5

print(f"O valor da sua viagem sera de {round(valor)}R$")

print()

print("aguarde...", end="\r")
time.sleep(2)
print(" " * 25, end="\r")

print(f"Ira demorar {tempo:.0f} minutos para o motorista chegar")

print()

time.sleep(1)

print("=-=" * 9)
print("\033[1;32mObrigado pela preferência!\033[m")
print("=-=" * 9)
print()
