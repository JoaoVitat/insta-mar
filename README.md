# main.py
import meumodulo

# 6.1 Soma
a = int(input("Digite o primeiro número: "))
b = int(input("Digite o segundo número: "))
print("Soma:", meumodulo.somar(a, b))

# 6.2 Verificar positivo ou negativo
num = int(input("Digite um número: "))
print(meumodulo.verificar_sinal(num))

# 6.3 Verificar maioridade
idade = int(input("Digite sua idade: "))
print(meumodulo.maioridade(idade))

