# Exercicio 1 #
import random

lista_aleatoria = [random.randint(1, 100) for _ in range(10)]
print("Lista de números aleatórios:", lista_aleatoria)


# Exercicio 2 #
lista_numeros = []

for i in range(3):
    numero = int(input(f"Digite o {i+1}º numero: "))
    lista_numeros.append(numero)
print("Numeros digitados:", lista_numeros)


# Exercicio 3 #
frase = input("Digite uma frase: ")
palavras = frase.split()
print("Palavras da frase:", palavras)


# Exercicio 4 #
lista_reversa = list(range(1, 11))
lista_reversa.reverse()
print("Lista reversa:", lista_reversa)


# Exercicio 5 #
palavras_teste = ["pedra", "papel", "tesoura", "Ordem", "Paranormal", "Desconjuracao"]
mais_longa = max(palavras_teste, key=len)
mais_curta = min(palavras_teste, key=len)
print("Palavra mais longa:", mais_longa)
print("Palavra mais curta:", mais_curta)


# Exercicio 6 #
pares = [x for x in range(1, 11) if x % 2 == 0]
impares = [x for x in range(1, 11) if x % 2 != 0]
lista_total = pares + impares
print("Lista combinada:", lista_total)


# Exercicio 7 #
numeros = list(range(1, 101))
pares_de_100 = [x for x in numeros if x % 2 == 0]
print("Numeros pares de 1 a 100:", pares_de_100)


# Exercicio 8 #
numeros = list(range(1, 11))
quadrado = [x**2 for x in numeros]
soma = sum(quadrado)
print("Quadrados de 1 a 10:", quadrado)
print("Soma dos quadrados:", soma)


# Exercicio 9 #
alfabeto = list("a, b, c, d, e, f, g, h, i, j, k, l, m, n, o, p, q, r, s, t, u, v, w, x, y, z")
random.shuffle(alfabeto)
letra = input("Escolha uma letra aleatoria: ").lower()
if letra in alfabeto:
    posicao = alfabeto.index(letra)
    chute = int(input(f"Em qual posicao você acha que a letra '{letra}' esta? (0-25): "))
    if chute == posicao:
        print("Acerto")
    else:
        print("Erro")
        
        
# Exercicio 10 #
# tentar fazer em outro vs para nao lotar esse #