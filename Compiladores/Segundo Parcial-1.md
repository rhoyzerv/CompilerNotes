Objetivos:

\-Informar de errores con claridad y exactitud  
\-Recuperarse del error y continuar  
\-No retrasar programas correctos

Algunos metodos de analisis sintáctico detectan el error lo antes posible (metodos LL y LR)

Algunas estrategias de recuperacion son:  
\-Modo panico: Adecuado para cuando no hay erorres multiples en la misma proposicion  
\-A nivel de la frase: Corregir con alguna cadena que permita continuar (.,;)  
\-Producciones de error  
\-Corrección global

**Gramáticas**  
Las reglas de cada lenguaje indican la sintaxis.  
La sintaxis puede especificarse mediante gramáticas libres de contexto (notación BNF - Backus-Naur Form)

Una gramatica permite evolución iterativa de un lenguaje  
\-Integra fácilmente nuevas construcciones  
Hay tres tipos de analizadores:  
\-Métodos Universales  
\-Métodos Descendentes: Construyen el árbol de la raiz a las hojas  
\-Ascendentes: Construyen el árbol de las hojas hacia la raiz

Gramatica LL LR  
LL (Descendente)  
LR (Ascendente)

La gramática anterior es LR utilizada para análisis ascendente, para e descendente no puede utilizarse porque es recursiva por a izquierda.  
Observe:  
<img width="475px;" height="210px;" src="../_resources/19b746b433cd3d8310e5706844efd46c-1" id="docs-internal-guid-2e577fda-7fff-8bb6-5073-d2e75bec9099" class="jop-noMdConv">

Existen métodos para eliminar la recursividad de este tipo de gramáticas obteniendo su equivalente:  
![58b9625a87d3b3058d4af25b212898d4.png](../_resources/58b9625a87d3b3058d4af25b212898d4-1.png)  
<br/>Ambiguedad  
Una gramática es ambigua si permite 2 o más árboles de análisis sintáctico para una mima expresión, suponga la gramática:  
<img width="674px;" height="89px;" src="../_resources/193e6a9d25f6976f8ad74e07bb87fba9-1" id="docs-internal-guid-1346ffad-7fff-1032-b93a-bd323cbf70f7" class="jop-noMdConv">

Gramatica libre de contexto:

\-Formalmente una gramática consiste en:  
\-Terminales (nombre del token- o simplemente token-)  
\-No terminales o variables sintácticas  
\-Un símbolo inicial en la primera producción  
\-Un conjunto de producciones

<img width="513px;" height="226px;" src="../_resources/7838a385a64c72e86269ffa459c01723-1" id="docs-internal-guid-5b55531b-7fff-917d-c653-57aab8f7ac44" class="jop-noMdConv">

![3c865e61be515d4032190d93c591e139.png](../_resources/3c865e61be515d4032190d93c591e139-1.png)

$$
E→E*E→-E*E→-id*E→-id*(E)→-id*(E+E)→-id*(id+id)
$$

![](blob:https://web.whatsapp.com/f1980b8d-8ffb-43c8-83d5-2b639b12d7e3)![](blob:https://web.whatsapp.com/f1980b8d-8ffb-43c8-83d5-2b639b12d7e3)![34eab17fe963b02ef3da34f9000ff48a.jpg](../_resources/34eab17fe963b02ef3da34f9000ff48a-1.jpg)  
<br/>Conversion de un AFN a Gramática

<img width="1065px;" height="260px;" src="../_resources/f8f1c8020950ece83abb45f33052a567-1" id="docs-internal-guid-0e67f63e-7fff-87ef-eeb5-00ba4f7d715d" class="jop-noMdConv">

**Derivacion:** Encontrar una cadena a partir del simbolo incial de la gramatica