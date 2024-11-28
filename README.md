# VLSI_PROYECTO_IV
## Parte 1. Sumador de un bit
La celda FAHDLLX0 tiene el siguiente esquemático

![image](https://github.com/user-attachments/assets/3c9c347e-7ee5-421a-acb8-47d122e7f2a4)

### Señal crítica y potencia
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
