# Actividad 3
## Problemas
1.  Determinar el promedio de calificaciones de un estudiante y si ha aprobado o no
``` Inicio
    Definir suma = 0
    Definir notas como lista vacía
    Imprimir "Ingresa el número de notas"
    Leer numnotas
    
    Para a desde 1 hasta numnotas hacer
        Imprimir "Ahora ingresa tu nota ", npta
        Leer nota
        Agregar nota a la lista de notas
    Fin Para
    
    Para cada nota en notas hacer
        suma = suma + nota
    Fin Para
    
    p = suma / numnotas
    Imprimir "Su promedio es de: ", p
    
    Si p >= 3.0 Entonces
        Imprimir "Felicitaciones, has aprobado"
    Sino
        Imprimir "Lo siento, no has pasado"
    Fin Si
Fin ```


2. Determinar la distancia total recorrida por un vehículo con registros de velocidad y tiempo
``` Inicio
    Definir distanciatotal = 0
    Definir velocidades, tiempos como listas vacías
    Imprimir "Ingresar el número de registros de velocidades y de tiempos"
    Leer numregistros
    
    Para a desde 1 hasta numregistros hacer
        Definir velocidad, tiempo
        Imprimir "Ingresar velocidad del registro ", velocidad, " en km/h"
        Leer velocidad
        Agregar velocidad a la lista de velocidades
        
        Imprimir "Ingresar tiempo del registro ", tiempo, " en hrs"
        Leer tiempo
        Agregar tiempo a la lista de tiempos
    Fin Para
    
    Para a desde 1 hasta numregistros hacer
        distanciatotal = distanciatotal + (velocidades[velocidad-1] * tiempos[tiempo-1])
    Fin Para
    
    Imprimir "Su distancia total recorrida es de:", distanciatotal, " km"
Fin ```

3. Calcular la edad de una persona a partir de su fecha de nacimiento y la fecha actual
``` Inicio
    Imprimir "Ingresar fecha de nacimiento (dd/mm/aa)"
    Leer ddnacimiento, mmnacimiento, aanacimiento
    
    Imprimir "Ingresar la fecha actual (dd/mm/aa)"
    Leer ddactual, mmactual, aaactual
    
    Definir edadaños = aaactual - aanacimiento
    Definir yacumplio como F
    
    Si mmactual > mmnacimiento Entonces
        yacumplio = V
    Sino Si mmactual = mmnacimiento Entonces
        Si ddactual >= ddnacimiento Entonces
            yacumplio = V
        Sino
            yacumplio = F
        Fin Si
    Sino
        yacumplio = F
    Fin Si
    
    Si yacumplio = F Entonces
        edadaños = edadaños - 1
    Fin Si
    
    Definir escumpleaños como F
    Si ddactual = ddnacimiento y mmactual = mmnacimiento Entonces
        escumpleaños = V
    Fin Si
    
    Si escumpleaños = V Entonces
        Imprimir "¡Felicitaciones, feliz cumpleaños!"
    Fin Si

    Imprimir "Edad calculada: ", edadaños, " años"
Fin ```
     


     
    