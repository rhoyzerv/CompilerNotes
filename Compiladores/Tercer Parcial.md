Un arbol de analisis sintactico puede construirse de raiz a hojas, pero tambien de hojas a raiz. Este es el caso del Analisis Sintactico ascendente por desplazamiento y reduccion, mejor conocido como LR, el proceso de construccion de hojas a raiz se le nombra reduccion de la cadena w para obtener el simbolo inicial de la gramatica.

Un mango es una subcadena que concuerda con el lado derecho de una produccion y cuya reduccion al no terminal del lado izquierdo representa un paso a la inversa de una derivacion por la derecha

Algunas gramaticas no pueden analizarse por desplazamiento y reduccion por tener conflicto en la accion, es decir, se debe desplazar o reducir (Conflicto de desplazamiento/reduccion) o no saber cual reduccion elegir (reduccion/reduccion)

&nbsp;-Una definición dirigida por la sintaxis son especificaciones de alto nivel para traducciones  
\-Los esquemas de traducción indican el orden de evaluación de las reglas semánticas  
\-Las definiciones y los esquemas de traducción revisan en un recorrido cada nodo del árbol sintáctico

Una regla semántica debe producir siempre el mismo resultado para cada cadena de entrada.

&nbsp;**Un compilador debe comprobar**  
\-Tipos de un operador u operando  
\-Flujo de control  
\-Break  
\-Unicidad  
\-Variables, casos  
\-Nombres  
\-En cierre de ciclos

**Bytecodes**

Opcode es el ensamblador de una máquina virtual  
Evita la dependencia de un Hardware específico  
Toma su nombre de la longitud que tiene cada operación  
Cada instrucción tiene un número de 0 a 255 seguido de parámetros  
Los parámetros son registros o direcciones de memoria  
Puede verse como código intermedio

![3097025e8353eb6c4993028db4dc168a.png](../_resources/3097025e8353eb6c4993028db4dc168a.png)

![2aaac3f011612364aa47c3e08b0b77f2.png](../_resources/2aaac3f011612364aa47c3e08b0b77f2.png)

&nbsp;![b0837674d65d65e10993aa3c8a0a2c15.png](../_resources/b0837674d65d65e10993aa3c8a0a2c15.png)

![2f73ffbbb93ce3d1dd7fcf5eb4d30f5d.png](../_resources/2f73ffbbb93ce3d1dd7fcf5eb4d30f5d.png)

**Analizador sintáctico LR**

\-Es un método general muy conocido que es igual de **eficiente** que otros métodos de desplazamiento / reducción

\-Un analizador LR encuentra el **primero error de la izquierda de la cadena**

\-Las gramáticas LR describen **más** lenguajes que las gramáticas LL

Un analizador sintáctico LR realiza las decisiones de desplazamiento-reducción mediante el mantenimiento de estados, para llevar el registro de la ubicación que tenemos en un análisis sintáctico.  
Los estados representan conjuntos de **“elementos”.**

&nbsp;

&nbsp;

&nbsp;