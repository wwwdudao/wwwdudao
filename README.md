# Função para somar
def add(x, y):
    return x + y

# Função para subtrair
def subtract(x, y):
    return x - y

# Função para multiplicar
def multiply(x, y):
    return x * y

# Função para dividir
def divide(x, y):
    if y == 0:
        return "Erro: Divisão por zero!"
    return x / y

# Escolha da operação
print("Selecione a operação:")
print("1 - Soma")
print("2 - Subtração")
print("3 - Multiplicação")
print("4 - Divisão")

# Entrada do usuário
choice = input("Digite a escolha (1/2/3/4): ")

num1 = float(input("Digite o primeiro número: "))
num2 = float(input("Digite o segundo número: "))

if choice == '1':
    print(f"{num1} + {num2} = {add(num1, num2)}")
elif choice == '2':
    print(f"{num1} - {num2} = {subtract(num1, num2)}")
elif choice == '3':
    print(f"{num1} * {num2} = {multiply(num1, num2)}")
elif choice == '4':
    print(f"{num1} / {num2} = {divide(num1, num2)}")
else:
    print("Opção inválida")
