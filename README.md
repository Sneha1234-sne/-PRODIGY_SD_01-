# PRODIGY_SD_01 
"A temperature conversion program, that converts Celsius to Fahrenheit and kelvin and present the converted values as outputs.""
def convert_temperature():
    # Prompt user for input temperature and unit
    temp = float(input("Enter the temperature: "))
    unit = input("Enter the unit of measurement (C for Celsius, F for Fahrenheit, K for Kelvin): ").upper()

    if unit == 'C':
        # Convert Celsius to Fahrenheit and Kelvin
        fahrenheit = (temp * 9/5) + 32
        kelvin = temp + 273.15
        print(f"{temp}°C is equivalent to {fahrenheit}°F and {kelvin}K.")
        
    elif unit == 'F':
        # Convert Fahrenheit to Celsius and Kelvin
        celsius = (temp - 32) * 5/9
        kelvin = celsius + 273.15
        print(f"{temp}°F is equivalent to {celsius}°C and {kelvin}K.")
        
    elif unit == 'K':
        # Convert Kelvin to Celsius and Fahrenheit
        celsius = temp - 273.15
        fahrenheit = (celsius * 9/5) + 32
        print(f"{temp}K is equivalent to {celsius}°C and {fahrenheit}°F.")
        
    else:
        print("Invalid unit entered. Please enter 'C', 'F', or 'K'.")

# Run the program
convert_temperature()
