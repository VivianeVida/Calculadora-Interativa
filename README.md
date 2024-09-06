# Calculadora-Interativa
## Calculadora Interativa
Esta é uma calculadora interativa em Python que permite ao usuário realizar operações básicas de adição, subtração, multiplicação e divisão em um loop contínuo até que o usuário decida sair.

## Função calculadora
def calculadora():
    while True:
        print("\nEscolha a operação:")
        print("1: Soma")
        print("2: Subtração")
        print("3: Multiplicação")
        print("4: Divisão")
        print("0: Sair")

        opcao = input("Digite o número da operação: ")

        if opcao == '0':
            print("Saindo...")
            break
        elif opcao in ['1', '2', '3', '4']:
            num1 = float(input("Digite o primeiro número: "))
            num2 = float(input("Digite o segundo número: "))

            if opcao == '1':
                resultado = num1 + num2
                print(f"Resultado: {num1} + {num2} = {resultado}")
            elif opcao == '2':
                resultado = num1 - num2
                print(f"Resultado: {num1} - {num2} = {resultado}")
            elif opcao == '3':
                resultado = num1 * num2
                print(f"Resultado: {num1} * {num2} = {resultado}")
            elif opcao == '4':
                if num2 != 0:
                    resultado = num1 / num2
                    print(f"Resultado: {num1} / {num2} = {resultado}")
                else:
                    print("Erro: Divisão por zero não é permitida.")
        else:
            print("Essa opção não existe. Tente novamente.")

calculadora()

## Descrição
A função calculadora permite ao usuário escolher uma operação matemática e inserir dois números para realizar a operação escolhida. O programa continua solicitando operações até que o usuário escolha sair.

## Funcionalidades
Soma: Adiciona dois números.
Subtração: Subtrai o segundo número do primeiro.
Multiplicação: Multiplica dois números.
Divisão: Divide o primeiro número pelo segundo, com verificação de divisão por zero.
Sair: Encerra o programa.

## Uso
Execute o script.
Escolha a operação desejada digitando o número correspondente.
Insira os dois números para a operação.
Veja o resultado da operação.
Repita o processo ou escolha “0” para sair.

## Exemplo de Uso
calculadora()

## Tratamento de Erros
O programa verifica se a opção escolhida é válida.
O programa verifica se a divisão por zero é tentada e exibe uma mensagem de erro apropriada.

 ## Requisitos
 Python 3.x

 ## Contribuições
 Contribuições são bem-vindas! Sinta-se à vontade para abrir uma issue ou enviar um pull request.

 ## Licença
 Este projeto está licenciado sob a Licença MIT - veja o arquivo LICENSE para mais detalhes.

