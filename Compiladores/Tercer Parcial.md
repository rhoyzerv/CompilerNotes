Un arbol de analisis sintactico puede construirse de raiz a hojas, pero tambien de hojas a raiz. Este es el caso del Analisis Sintactico ascendente por desplazamiento y reduccion, mejor conocido como LR, el proceso de construccion de hojas a raiz se le nombra reduccion de la cadena w para obtener el simbolo inicial de la gramatica.

Un mango es una subcadena que concuerda con el lado derecho de una produccion y cuya reduccion al no terminal del lado izquierdo representa un paso a la inversa de una derivacion por la derecha

Algunas gramaticas no pueden analizarse por desplazamiento y reduccion por tener conflicto en la accion, es decir, se debe desplazar o reducir (Conflicto de desplazamiento/reduccion) o no saber cual reduccion elegir (reduccion/reduccion)

[3Parcial_Compiladores.ods](../_resources/3Parcial_Compiladores.ods)