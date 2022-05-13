# First
- Primeiro repositório feito com o propósito de aprender sobre o GitHub (Não pretendo apagar-lo)

# Copie o Código
```
i = s = c = count = count2 = count3 = count4 = 0
while True:
    count4 += 1
    print("\033[1;33m-\033[m" * 40)
    print("\033[1;36mCADASTRE UMA PESSOA\033[m")
    print("\033[1;33m-\033[m" * 40)
    i = int(input("Idade: "))
    s = str(input("Sexo [M/F]: "))[0].lower()
    while True:
        if s == "m" or s == "f":
            break
        if s != "m" or s != "f":
            print("-" * 40)
            print("\033[1;31mCertifique-se de que digitou corretamente\033[m")
            print("-" * 40)
            s = str(input("Sexo[M/F]: "))
    if i > 18:
        count += 1
    if s == "m":
        count2 += 1
    if s == "f" and i < 20:
        count3 += 1
    c = str(input("Você quer continuar cadastrando [S/N]? "))[0].lower()
    while True:
        if c == "s" or c == "n":
            break
        if c != "s" or c != "n":
            print("-" * 40)
            print("\033[1;31mCertifique-se de que digitou corretamente\033[m")
            print("-" * 40)
            c = str(input("Você quer continuar cadastrando [S/N]? "))[0].lower()
    if c == "n":
        print("\033[1;34m-\033[m" * 40)
        print("\033[1;35mObrigado por usar o programa de cadastro! volte sempre.\033[m")
        print("\033[1;34m-\033[m" * 40)
        break
if count == 1:
    print("Ao todo tem 1 única pessoa com mais de 18 anos cadastrada.")
if count == 0:
    print("Nenhuma pessoa com mais de 18 anos foi cadastrada")
if count != 0 and count != 1:
    print("Ao todo tem {} pessoas com mais de 18 anos cadastradas.".format(count))
if count2 == 1:
    print("Só foi cadastrado 1 homem.")
if count2 == 0:
    print("Nenhum homem foi cadastrado.")
if count2 != 0 and count2 != 1:
    print("Foram cadastrados {} homens no total.".format(count2))
if count3 == 1:
    print("Só tem 1 mulher com menos de 20 anos cadastrada.")
if count3 == 0:
    print("Nenhuma mulher com menos de 20 anos foi cadastrada.")
if count3 != 0 and count3 != 1:
    print("Foram cadastradas {} mulheres com menos de 20 anos.".format(count3))
if count4 == 1:
    print("No total foi cadastrada {} pessoa.".format(count4))
if count4 != 1:
    print("No total foram {} pessoas cadastradas".format(count4))
```
