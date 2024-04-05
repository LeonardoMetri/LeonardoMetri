- 👋 Hi, I’m @LeonardoMetri
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
LeonardoMetri/LeonardoMetri is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
---> def adicao(a, b):
    return a + b

def subtracao(a, b):
    return a - b

def multiplicacao(a, b):
    return a * b

def divisao(a, b):
    if b != 0:
        return a / b
    else:
        return "Erro: Divisão por zero"

def menu():
    print("Escolha a operação:")
    print("1 - Adição")
    print("2 - Subtração")
    print("3 - Multiplicação")
    print("4 - Divisão")
    print("0 - Sair")

def calculadora():
    while True:
        menu()
        opcao = input("Digite o número da operação desejada: ")

        if opcao == '0':
            print("Encerrando a calculadora.")
            break
        elif opcao in ('1', '2', '3', '4'):
            num1 = float(input("Digite o primeiro número: "))
            num2 = float(input("Digite o segundo número: "))
            if opcao == '1':
                print("Resultado:", adicao(num1, num2))
            elif opcao == '2':
                print("Resultado:", subtracao(num1, num2))
            elif opcao == '3':
                print("Resultado:", multiplicacao(num1, num2))
            elif opcao == '4':
                print("Resultado:", divisao(num1, num2))
        else:
            print("Opção inválida. Por favor, escolha uma opção válida.")
