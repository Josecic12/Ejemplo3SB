# Ejemplo3SB
Repositorio de prueba de estructura de datos
def fibonacci_recursive(n):
    if n <= 0:
        return []
    elif n == 1:
        return [0]
    elif n == 2:
        return [0, 1]
    else:
        sequence = fibonacci_recursive(n - 1)
        next_number = sequence[-1] + sequence[-2]
        sequence.append(next_number)
        return sequence

n = 10
result = fibonacci_recursive(n)
print(result)
