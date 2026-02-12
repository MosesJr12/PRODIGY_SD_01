def celsius_to_fahrenheit(c):
    return (c * 9/5) + 32

def celsius_to_kelvin(c):
    return c + 273.15

def fahrenheit_to_celsius(f):
    return (f - 32) * 5/9

def fahrenheit_to_kelvin(f):
    return (f - 32) * 5/9 + 273.15

def kelvin_to_celsius(k):
    return k - 273.15

def kelvin_to_fahrenheit(k):
    return (k - 273.15) * 9/5 + 32


print("Temperature Conversion Program")
print("1. Celsius")
print("2. Fahrenheit")
print("3. Kelvin")

choice = int(input("Choose the input unit (1/2/3): "))
temp = float(input("Enter the temperature value: "))

if choice == 1:
    print("Fahrenheit:", celsius_to_fahrenheit(temp))
    print("Kelvin:", celsius_to_kelvin(temp))

elif choice == 2:
    print("Celsius:", fahrenheit_to_celsius(temp))
    print("Kelvin:", fahrenheit_to_kelvin(temp))

elif choice == 3:
    print("Celsius:", kelvin_to_celsius(temp))
    print("Fahrenheit:", kelvin_to_fahrenheit(temp))

else:
    print("Invalid choice!")
