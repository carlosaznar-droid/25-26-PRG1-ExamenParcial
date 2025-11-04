# Examen Parcial - carlosaznar-droid

**Usuario GitHub:** carlosaznar-droid
**Fecha:** 4 de noviembre de 2025
**Retos tenidos en cuenta:** Reto 003

---

## Instrucciones

A continuación encontrarás fragmentos de código extraídos de tus entregas. Cada fragmento contiene una o más situaciones relacionadas con los conceptos vistos en clase.

Para cada pregunta debes:
1) Identificar a qué se refiere la observación
2) Explicar si es o no un error y por qué
3) Proponer la corrección

Nota: Responde 5 de las 8 preguntas (en función a lo indicado en el examen).


---

## Pregunta 1

Archivo: `Reto3.java` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/3b54c071dd690f3d9fab8141edc9b686d7cd498d/entregas/AznarCarlos/reto-003/Reto3.java) (Reto 003)

```java
final String SEPARADOR = "[   ]";
final String TECHO = "||   |   |###|   |   ||";
```

¿Qué observas en este código?

---

## Pregunta 2

Archivo: `Reto3.java` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/3b54c071dd690f3d9fab8141edc9b686d7cd498d/entregas/AznarCarlos/reto-003/Reto3.java) (Reto 003)

```java
for (int hora = 0; hora < 24; hora++) {
    System.out.println("Son las " + hora + ":00 del día " + dia);
    for (int i = 0; i < 1; i++) {
        System.out.println(TECHO);
    }
}
```

¿Qué observas en este código?

---

## Pregunta 3

Archivo: `Reto3.java` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/3b54c071dd690f3d9fab8141edc9b686d7cd498d/entregas/AznarCarlos/reto-003/Reto3.java) (Reto 003)

```java
System.out.print(
    !abierta ? (encendida ? VENTANA_CERRADA : VENTANA_ABIERTA_CON_LUZ)
             : VENTANA_ABIERTA_SIN_LUZ);
```

¿Qué observas en este código?

---

## Pregunta 4

Archivo: `Reto3.java` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/3b54c071dd690f3d9fab8141edc9b686d7cd498d/entregas/AznarCarlos/reto-003/Reto3.java) (Reto 003)

```java
for (int planta = 1; planta <= 7; planta++) {
    for (int columna = 1; columna <= 6; columna++) {
        // ...
        if (columna == 3) {
            System.out.print(SEPARADOR);
        }
    }
    System.out.println();
}
```

¿Qué observas en este código?

---

## Pregunta 5

Archivo: `Reto3.java` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/3b54c071dd690f3d9fab8141edc9b686d7cd498d/entregas/AznarCarlos/reto-003/Reto3.java) (Reto 003)

```java
public class Reto3{
    // ...
}
```

¿Qué observas en este código?

---

## Pregunta 6

Archivo: `Reto3.java` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/3b54c071dd690f3d9fab8141edc9b686d7cd498d/entregas/AznarCarlos/reto-003/Reto3.java) (Reto 003, líneas 28-31)

```java
System.out.print(
        !abierta ? (encendida ? VENTANA_CERRADA : VENTANA_ABIERTA_CON_LUZ)
                : VENTANA_ABIERTA_SIN_LUZ);
```

¿Qué observas en este código?

---

## Pregunta 7

Archivo: `Reto3.java` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/3b54c071dd690f3d9fab8141edc9b686d7cd498d/entregas/AznarCarlos/reto-003/Reto3.java) (Reto 003, líneas 18-22)

```java
for (int i = 0; i < 1; i++) {
    System.out.println(TECHO);

}
```

¿Qué observas en este código?

---

## Pregunta 8

Archivo: `Reto3.java` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/3b54c071dd690f3d9fab8141edc9b686d7cd498d/entregas/AznarCarlos/reto-003/Reto3.java) (Reto 003, líneas 5-7)

```java
final double PERSIANA_ABIERTA = 0.7;
final double LUZ_ENCENDIDA = 0.6;
```

¿Qué observas en este código?

RESULTADO 

# Examen Parcial
## Pregunta 2
---
```java 
for (int hora = 0; hora < 24; hora++) {
    System.out.println("Son las " + hora + ":00 del día " + dia);
    for (int i = 0; i < 1; i++) {
        System.out.println(TECHO);
    }
}
```
Uno de los problemas que podemos observar a los ojos de un ingeniero es que dentro de este bloque de codigo observamos el uso de un bucle ```for``` para la asignacion de la hora que sera expuesta a la hora de la ejecucion del mismo, a su vez vemos unas variables en camel case es decir que estas son declaraciones ````int```` y que no son ````final```` ya que alternan su resultado, la variable ````dia```` no esta declarada es decir que no se le ha asignado un valor como en el caso de ````hora````,su solucion seria asignarla antes del bucle propuesto. Otro error q podemos observar es la variable de ``TECHO`` algo que podriamos ver es la nomenclatura expuesta screaming snake case es decir que esta variable no declarada deberia estar compuesta por un ``final String``+``TECHO`` y luego el valor que hayamos propuesto. Con estos problemas resueltos miramos el codigo y nos daria a entender que la funcion del mismo es valorar la condicion y ejecutar su incremento para realizar una secuencia indefinida. Viendo la segunda parte del codigo es decir el segundo ``for`` miramos ese bloque en el que podemos entender que se quiere procesar una variable ``final String``es decir ``TECHO`` es el bucle inecesario que se procesa  ``for (int i = 0; i < 1; i++) ``esta parte del bloque la podriamos indicar como inecesaria para corregirlo bastaria con imprimirlo antes del codigo 

---
## Pregunta 3
 
````
 System.out.print(
    !abierta ? (encendida ? VENTANA_CERRADA : VENTANA_ABIERTA_CON_LUZ)
             : VENTANA_ABIERTA_SIN_LUZ); 
````
En este fragmento de codigo vemos la aplicacion de ternarios como es el ````boolean```` usado para interaciones que solo pueden ser true o false, en este caso se tiene en cuenta mas de un caso es decir una ventada cerrada con luz o sin luz y una ventana abierta con luz o sin luz a la hora de leerlo puede llegar a ser un tanto contradictorio es verdad que dentro de este reto se pedia que aunque este cerrada se diera a entender que, la ventana por detras tuviese o no luz. Al compilar este codigo podemos destacar un error de escritura o mas bien de entendimiento ya que cuando se ejecuta tiene un problema lógico cuando la ventana está cerrada y la luz está apagada, imprime ````VENTANA_ABIERTA_CON_LUZ````
lo cual como decia antes llega a ser un tanto contradictorio la solucion sin llegar a utilizar un ```if/else```seria 
```` 
java

System.out.print(
    !abierta
        ? (encendida ? VENTANA_CERRADA_CON_LUZ : VENTANA_CERRADA_SIN_LUZ)
        : (encendida ? VENTANA_ABIERTA_CON_LUZ : VENTANA_ABIERTA_SIN_LUZ));
````
lo que ejecutaria esta parte seria,

 Si la ventana esta cerrada ``!abierta`` 	
Si la luz esta encendida - imprime ``VENTANA_CERRADA_CON_LUZ``
Si la luz esta apagada - imprime ``VENTANA_CERRADA_SIN_LUZ``
Si la ventana esta abierta:  
 	Si la luz esta encendida → imprime ``VENTANA_ABIERTA_CON_LUZ``
Si la luz esta apagada - imprime ``VENTANA_ABIERTA_SIN_LUZ``
con ese fragmento corregido el codigo pasaria a ser mas limpio y entendible al usuario que desconozca del tema, aunque si busca algo menos complejo podrias emplear el ````if/else````

---
## Pregunta 4
````
for (int planta = 1; planta <= 7; planta++) {
    for (int columna = 1; columna <= 6; columna++) {
        // ...
        if (columna == 3) {
            System.out.print(SEPARADOR);
        }
    }
    System.out.println();
}

````
Esto es otro fragmento del codigo y a simple vista podriamos decir que se ve un bloque ded codigo divido en partes la primera seria la asignacion de las variable ````planta y columna```` y como se puede ver este fragmento no tiene errores ya que dentro del bucle ````for/if```` vemos cada unas de las variables int en nomenclatura snake case y se plantea el if para imprimir sin saltar linea una variable ``final String`` en Screaming snake case. Este codigo no tiene errores pero como recomendacion seria mejor aplicar utilizar metodos para que se vean mas limpio y entendible 

---
## Pregunta 5

````
public class Reto3{
    // ...
}
````
Otro fragmento que podriamos decir que no tiene errores pero efectivamente posee alguno como si el reto requiere que el programa se ejecute desde esta clase entonces debería incluir el método ````main```` su correcion seria poner 
````
public static void main(String[] args) {
}
````
pero seguramente este ya este puesto en el codigo y no sea necesario corregirlo por lo que si efectivamente el codigo esta bien aunque para que sea mas limpio deberiamos poner ````reto3```` en vez de ````Reto3````

--- 

## Pregunta 8
````
final double PERSIANA_ABIERTA = 0.7;
final double LUZ_ENCENDIDA = 0.6;
````
En este segmento de codigo podemos ver la asignacion de dos variables de ``double`` en ``final`` que indican una probabilidad que poxteriormente seran asignadas con un ``math.random`` este codigo esta biene escrito y no se puede poner mas limpio ya que el unico erro que podriamos ver seria la nomenclatura pero esta bien expuesta ya que esta en ``screaming snake case`` y no se puede hacer mas aunque podriamos cambiar el nombre para que sea mas entendible
