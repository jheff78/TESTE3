Vou mostrar três formas de fazer isso usando os três laços de repetição comuns em Python: for, while, e do-while (este último emulada). Em todas as soluções, a contagem é feita de 20 a 1 e o número 13 é pulado.

1. Usando for
python
Copiar código
for andar in range(20, 0, -1):
    if andar == 13:
        continue
    print(andar)
2. Usando while
python
Copiar código
andar = 20
while andar > 0:
    if andar != 13:
        print(andar)
    andar -= 1
3. Usando uma estrutura do-while emulada com while
Como Python não tem um laço do-while, podemos emular o comportamento:

python
Copiar código
andar = 20
while True:
    if andar != 13:
        print(andar)
    andar -= 1
    if andar == 0:
        break
Esses códigos imprimem todos os números dos andares em ordem decrescente, exceto o 13.
