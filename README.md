📘 Avaliação A1 – Técnicas de Desenvolvimento de Algoritmos

Este repositório contém quatro programas desenvolvidos em Python para a Avaliação A1 da disciplina Técnicas de Desenvolvimento de Algoritmos.
 Cada exercício aborda um conceito essencial visto em aula: Estruturas Condicionais, Estruturas de Repetição, Listas e Dicionários.
 
🧩 01. Estruturas Condicionais – Classificação de Temperatura

Arquivo: 1-estruturas-condicionais/classificacao_temperatura.py

Este programa solicita que o usuário digite uma temperatura em graus Celsius e, usando if / elif / else, classifica o clima como:
Frio → temperatura abaixo de 15


Agradável → entre 15 e 25


Quente → acima de 25


📌 Código utilizado:
# Programa para classificar a temperatura informada pelo usuário

# Entrada: o usuário digita a temperatura em graus Celsius
temperatura = float(input("Digite a temperatura em graus Celsius: "))

# Estrutura condicional para classificar a temperatura
if temperatura < 15:
    print("Clima frio.")
elif temperatura >= 15 and temperatura <= 25:
    print("Clima agradável.")
else:
    print("Clima quente.")


🔁 02. Estruturas de Repetição

Pasta: 2-estruturas-repeticao/

Programas que exibem números pares de 1 a 100, utilizando dois tipos de laço:
 ✔ for
 ✔ while

2.1 – Usando FOR
Arquivo: pares_for.py
# Imprime números pares de 1 a 100 usando for

for numero in range(1, 101):
    # Verifica se o número é par
    if numero % 2 == 0:
        print(numero)


2.2 – Usando WHILE
Arquivo: pares_while.py
# Imprime números pares de 1 a 100 usando while

numero = 1  # Começa no 1

while numero <= 100:
    # Se o número for par, imprime
    if numero % 2 == 0:
        print(numero)
    
    numero += 1  # Incrementa o contador


📝 03. Listas – Cadastro de Alunos

Arquivo: 3-listas/cadastro_alunos.py

Programa que permite ao usuário digitar nomes de alunos até escrever "sair".
 Todos os nomes digitados são armazenados em uma lista, que é exibida ao final.
📌 Código utilizado:
# Programa para armazenar nomes de alunos em uma lista

lista_alunos = []  # Lista vazia para guardar os nomes

while True:
    nome = input("Digite o nome do aluno (ou 'sair' para finalizar): ")

    # Condição para encerrar o cadastro
    if nome.lower() == "sair":
        break

    # Adiciona o nome digitado na lista
    lista_alunos.append(nome)

# Exibe todos os alunos cadastrados
print("\nLista de alunos cadastrados:")
for aluno in lista_alunos:
    print(aluno)


🛒 04. Dicionários – Cadastro de Produtos

Arquivo: 4-dicionarios/cadastro_produtos.py

Programa que cadastra produtos contendo nome e preço, armazenando cada produto em um dicionário.
 Todos os dicionários são armazenados em uma lista, que é exibida ao final.
📌 Código utilizado:
# Programa para cadastrar produtos usando dicionários

lista_produtos = []  # Lista que vai armazenar vários dicionários

while True:
    nome_produto = input("Digite o nome do produto (ou 'sair' para finalizar): ")

    # Condição para encerrar
    if nome_produto.lower() == "sair":
        break

    # Recebe o preço do produto
    preco_produto = float(input("Digite o preço do produto: "))

    # Cria um dicionário com nome e preço
    produto = {
        "nome": nome_produto,
        "preco": preco_produto
    }

    # Adiciona o dicionário na lista
    lista_produtos.append(produto)

# Exibe todos os produtos cadastrados
print("\nLista de produtos cadastrados:")
for item in lista_produtos:
    print(f"Produto: {item['nome']} | Preço: R$ {item['preco']}")


▶️ Como Executar os Programas
Certifique-se de ter o Python 3 instalado.


Abra o terminal na pasta do exercício.


Execute:


python arquivo.py

Exemplo:
python classificacao_temperatura.py
