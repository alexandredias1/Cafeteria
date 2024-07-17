# Cafeteria

Este é um script em Python que simula o processo de seleção e preparo de diferentes tipos de café em uma cafeteria. O usuário pode escolher entre várias opções de café e o script simula o tempo de preparo antes de informar que o café está pronto.

## Descrição

O script apresenta um menu para o usuário selecionar um tipo de café. Dependendo da escolha, o script simula o tempo de preparo do café usando a função `time.sleep()` para criar uma contagem regressiva. O usuário pode continuar escolhendo cafés ou encerrar o programa.

## Funcionalidades

- Seleção de diferentes tipos de café:
  - Expresso
  - Tradicional
  - Cappuccino
  - Latte
  - Descafeinado
- Simulação do tempo de preparo para cada tipo de café.
- Possibilidade de encerrar o programa a qualquer momento.

## Como usar

1. Certifique-se de ter o Python instalado em seu sistema.
2. Salve o script em um arquivo com a extensão `.py` (por exemplo, `cafeteria.py`).
3. Abra um terminal ou prompt de comando.
4. Navegue até o diretório onde o script foi salvo.
5. Execute o script com o comando `python cafeteria.py`.
6. Siga as instruções na tela para selecionar o café desejado e aguarde a simulação do tempo de preparo.

## Exemplo de uso

```python
import time

cafe = int(input("Escolha o seu café\n1 - Expresso\n2 - Tradicional\n3 - Cappuccino\n4 - Latte\n5 - Descafeinado\n6 - Para encerrar o programa: "))

while True:

    if cafe == 1:
        for coffe1 in range(1, 11):
            print(f"O café estará pronto em 10s {coffe1}")
            time.sleep(1)
        print("O café Expresso está pronto!")
        cafe = int(input("Escolha o seu café\n1 - Expresso\n2 - Tradicional\n3 - Cappuccino\n4 - Latte\n5 - Descafeinado\n6 - Para encerrar o programa: ")) 

    elif cafe == 2:
        for coffe2 in range(1, 16):
            print(f"O café estará pronto em 15s {coffe2}")
            time.sleep(1)
        print("O café Tradicional está pronto!")
        cafe = int(input("Escolha o seu café\n1 - Expresso\n2 - Tradicional\n3 - Cappuccino\n4 - Latte\n5 - Descafeinado\n6 - Para encerrar o programa: ")) 
        
    elif cafe == 3:
        for coffe3 in range(1, 23):
            print(f"O café estará pronto em 22s {coffe3}")
            time.sleep(1)
        print("O café Cappuccino está pronto!")
        cafe = int(input("Escolha o seu café\n1 - Expresso\n2 - Tradicional\n3 - Cappuccino\n4 - Latte\n5 - Descafeinado\n6 - Para encerrar o programa: ")) 
        
    elif cafe == 4:
        for coffe4 in range(1, 19):
            print(f"O café estará pronto em 18s {coffe4}")
            time.sleep(1)
        print("O café Latte está pronto!")
        cafe = int(input("Escolha o seu café\n1 - Expresso\n2 - Tradicional\n3 - Cappuccino\n4 - Latte\n5 - Descafeinado\n6 - Para encerrar o programa: ")) 

    elif cafe == 5:
        for coffe5 in range(1, 21):
            print(f"O café estará pronto em 20s {coffe5}")
            time.sleep(1)
        print("O café Descafeinado está pronto!")
        cafe = int(input("Escolha o seu café\n1 - Expresso\n2 - Tradicional\n3 - Cappuccino\n4 - Latte\n5 - Descafeinado\n6 - Para encerrar o programa: "))

    elif cafe == 6:
        print("Programa encerrado.")
        break
    else:
        print("Opção inválida")
        break 
