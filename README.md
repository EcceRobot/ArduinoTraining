# ArduinoTraining

## Software Links

### Processing
https://processing.org/download 

### Arduino IDE
https://www.arduino.cc/en/software




double tempK = log(known_resistor_ohm * ((known_Vcc / analogInput_voltage - 1)));
tempK = 1 / (0.001129148 + (0.000234125 + (0.0000000876741 * tempK * tempK )) * tempK );    // Temp Kelvin  
float tempC = tempK - 273.15;                                                               // Convert Kelvin to Celcius
float tempF = (tempC * 9.0)/ 5.0 + 32.0;                                                    // Convert Celcius to Fahrenheit
