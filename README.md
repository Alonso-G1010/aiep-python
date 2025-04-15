temperaturas = []

for i in range(7):
    while True:
        try:
            temperatura = float(input(f"Ingrese la temperatura del día {i+1}: "))
            temperaturas.append(temperatura)
            break
        except ValueError:
            print("Por favor, ingresa un número válido.")

promedio = sum(temperaturas) / len(temperaturas)
maxima = max(temperaturas)
minima = min(temperaturas)

print(f"\nResultados:")
print(f"Temperaturas ingresadas: {temperaturas}")
print(f"Promedio de las temperaturas: {promedio:.2f}°C")
print(f"Temperatura máxima: {maxima}°C")
print(f"Temperatura mínima: {minima}°C")
