Gastos de persona mes a mes
``` Inicio
    Imprimir "Ingrese el valor de la compra", compra
    Leer compra
    
    Imprimir "Ingrese la tasa de interés anual(%)", tasafija
    Leer tasafija

    Imprimir "Ingrese el número de cuotas", cuotas
    Leer cuotas
    
        Convertir tasa anual a tasa mensual
        tasamensual=tasafija/12/100

        Calcular cuotamensual
        cuotamensual=(compra*tasamensual)/(1-(1+tasamensual)^-cuotas)

        Imprimir valorcuota mes a mes
        Definir totalpago=0
        
        Para pagomensual hacer
            pagomensual=cuotamensual
            totalpago=totalpago+pagomensual
        Fin Para
        Leer gasto total
        Imprimir "El gasto total es de:", gastotal
Fin ```


