# VLSI_PROYECTO_IV
Kender Ortiz y Josué Quirós

## Parte 1. Sumador de un bit
La celda FAHDLLX0 tiene el siguiente esquemático

![image](https://github.com/user-attachments/assets/3c9c347e-7ee5-421a-acb8-47d122e7f2a4)

### 1.1 Señal crítica y potencia
Para determinar la señal crítica del sumador se realiza la simulación para ver como el cambio en las entradas afecta las señales de salida

![image](https://github.com/user-attachments/assets/b65bd10f-5857-4e10-a600-4319a9f0a4c0)

Se realiza mide para cada entrada con las otras 2 constantes y se obtiene los siguiente valores

| Entrada | Transición | Retardo en S (ps)| Retardo en C0 (ps)|
|---------|------------|------------------|-------------------|
| A       | 0 → 1      | 243              | 252               |
| A       | 1 → 0      | 537              | 397               |
| B       | 0 → 1      | 225              | 248               |
| B       | 1 → 0      | 511              | 377               |
| Ci      | 0 → 1      | 207              | 221               |
| Ci      | 1 → 0      | 455              | 309               |

![image](https://github.com/user-attachments/assets/469e101b-c3f5-4f93-ae5f-f9e7a11eade3)

Para hacer el calculo de potencia se realiza una simulación donde se respeta el tiempo de retardo maximo y se calcula la corriente promedio de vdd a lo lardo de la prueba.
Lo que nos da un P = 20.8 $\mu A$ * 1.8 $V$ = 36 $\mu W$

![image](https://github.com/user-attachments/assets/c8fb99a7-d4e6-490f-9b8d-d1d45bbf992c)

## Parte 2. Registro de un bit

EL esqueamtico de la compuerta DFFHDLX0 

![image](https://github.com/user-attachments/assets/8d7ecdf3-bf42-4e46-8749-6c73cbd4d013)


Para determinar la señal crítica del registro se realiza la simulación para ver como el cambio en las entradas afecta las señales de salida. Esto se mide apartir de un posedge del relog, una vez que D cambia.

| Entrada | Transición | Retardo en Q (ps)| Retardo en QN (ps)|
|---------|------------|------------------|-------------------|
| D       | 0 → 1      | 499              | 586               |
| D       | 1 → 0      | 499              | 586               |

![image](https://github.com/user-attachments/assets/1968556a-4b12-4312-93bf-8854c8740f81)

Esto lo que nos indica que el periodo del clock máximo es aproximadamente 1.71 ns (584.8 MHz)

## Parte 3. Trazado de las compuertas simples

### El layout de la compuerta FAHDLLX0

![image](https://github.com/user-attachments/assets/ec51ae8a-df22-4255-81dd-49b4b2824aff)

### El layout de la compuerta DFFHDLX0

![image](https://github.com/user-attachments/assets/eeaf4961-a4be-4716-83fb-79bde15ab25b)

### Circuito completo

![image](https://github.com/user-attachments/assets/dc7a1a2b-1f07-4b67-bf8c-f265680d550b)

