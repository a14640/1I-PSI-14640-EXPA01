<h3> # 1I-PSI-14640-EXPA01</h3>    

Aqui esta o codigo do jogo

import random
print("----------------GUESS THE NUMBER----------------")
tentativas = int(6)
nome = input("Insira o seu Nick: ")
SecretN = random.randint(0,20)

while tentativas > 0:
  numero = int(input("Insira um valor: "))
  if numero == SecretN:
    print("---Acertaste---")
    exit()
  elif numero < SecretN:
    print("---Número inferior---")
    tentativas -= 1
    print(f"Restam {tentativas} tentativas.")
  elif numero > SecretN:
    print("---Número superior---")
    tentativas -= 1
    print(f"Restam {tentativas} tentativas.")

print(f"As tentativas acabaram e o número correto é {SecretN} .")




