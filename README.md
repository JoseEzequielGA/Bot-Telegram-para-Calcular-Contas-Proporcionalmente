# 💰 Calculadora de Conta Proporcional

Projeto desenvolvido para estudar, meu nivel de python é iniciante por esse motivo o codigo esta escrito de maneira mais simples, todo o processo fora a criação do codigo em python foi com auxilio da IA Gemini.

A solução foi desenvolvida tanto como um **script Python** quanto como um **bot para Telegram**.

## 🎯 Conceito e Funcionamento

A lógica do projeto é replicar a fórmula de divisão proporcional usada na minha planilhas de controle financeiro pessoal:

1.  Calcular o valor recebido por duas pessoas.
2.  Com base no valor da conta, retorna o valor que cada um deve pagar proporcionalmente.

**Exemplo:**

  * Salário 1: R$ 1.000,00
  * Salário 2: R$ 3.000,00
  * Valor da Conta: R$ 987
  * Pessoa 1:  25% da conta | R$ 246,75
  * Pessoa 2:  75% da conta | R$ 740,25


## 💻 Script Python (Criado por Mim)

O script original

 ``` python
def linha():
    print("=" * 37)



salario_1 = int(input("Insira o primeiro sálario: "))
salario_2 = int(input("Insira o Segundo Sálario: "))

conta_1 = (salario_1 / (salario_1 + salario_2) * 100)
conta_2 = (salario_2 / (salario_2 + salario_1) * 100)


print("=" * 20)
print("Separador de Contas Proporcional")
print("=" * 20)
print( "Pessoa 1 paga: " f"{(round((conta_1),2))} %")
print( "Pessoa 2 paga: " f"{(round((conta_2),2))} %")

Valor_conta = int(input("Valor da conta a ser paga: "))

print("=" * 20)
print("Valor da Conta: " , Valor_conta)
print("Pessoa 1 paga: " ,(round((conta_1 / 100 * Valor_conta),2)))
print("Pessoa 2 paga: " ,(round((conta_2 / 100 * Valor_conta),2)))
 ```


**Saída :**

```
=====================================
Separador de Contas Proporcional
====================
Pessoa 1 paga: 85.71 %
Pessoa 2 paga: 14.29 %
====================
Valor da Conta:  988
Pessoa 1 paga:  846.86
Pessoa 2 paga:  141.14
```

## 🤖 Bot para Telegram

Achei que seria interessante ter esse código de maneira simples e de facil acesso, então joguei o meu código no Gemini e 
segui o passa a passo para criação desse Bot.

### 🛠️ Tecnologias Utilizadas

  * **Python**
  * Biblioteca `python-telegram-bot`
  * Hospedagem em serviço como **Replit**

### 💬 Exemplo de Interação

A interação com o bot será como no exemplo a seguir:

> **Usuário:** `1200,2000,890`
> **Bot:**
> Pessoa 1 paga: R$ 333.75 (37.5 %)
> Pessoa 2 paga: R$ 556.25 (62.5 %)


## 🧑‍💻 Autor

Jose Alves

[LinkedIn]([https://linkedin.com/in/SEU_USER_LINKEDIN](https://www.linkedin.com/in/jose-alves-348122230/)) 🔗




> <span style="color:red;">**ATENÇÃO:**</span> `O bot não está disponivel para uso, foi apenas um projeto para estudo!`
