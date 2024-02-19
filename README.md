# Validador_da_sequ-ncia_de_Fibonacci

def is_fibonacci_number(n):
    a, b = 0, 1

    
    if n == 0:
        return True

    while b < n:
        a, b = b, a + b
        if b == n:
            return True


# Exemplo de uso
numero_informado = int(input("Informe um número: "))

if is_fibonacci_number(numero_informado):
    print(f"{numero_informado} pertence à sequência de Fibonacci.")
else:
    print(f"{numero_informado} não pertence à sequência de Fibonacci.")
