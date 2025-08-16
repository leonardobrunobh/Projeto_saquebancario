# Projeto_saquebancario
Um pequeno e simples script que remonta uma especie de saque no caixa eletronico.

import time
saldo = 2000
saque_maximo = 500   #variáveis globais
limite_saque = 0

## abaixo está o menu de abertura do banco com as opções

opcao = int(input("""

    Bem Vindo ao seu Banco Virtual \n
    
    Escolha uma opcao \n

    ======== MENU ===========
    
            [1] Saque \n
            [2] Saldo \n
            [3] Extrato \n
            [4] Deposito \n
            [5] Sair \n

    ========================\n"""
))

## essa é a opção do saque
if limite_saque <=3:
    if opcao == 1:
        limite_de_saque = limite_saque + 1
        saque = int(input("Qual o valor deseja sacar? "))
            if saque <= saque_maximo and saque <= saldo:
        
                print("\n Seu saque está sendo processado \n")
                saldo = saldo - saque

                time.sleep(4)
                print("Retire o seu dinheiro na boca do caixa. \n")
else: 
    print(" Você excedeu o limite de saques diários. \n")


##essa é a opção de exibição do saldo
elif opcao == 2:
    print("O seu saldo é", saldo)


elif opcao == 3:
    print

else:
    print("Opção inválida")



