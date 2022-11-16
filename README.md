# PII Full GRASP and SOLID
## FIT
### Universidad Católica del Uruguay

En este programa trabajaremos con recetas de cocina que involucran ingredientes y equipamiento.

## Solución
Se aplica DIP, haciendo que ahora IPrinter, y sus implementaciones, dependan de una interfaz IRecipe, podiendo así sustituir IRecipe por cualquier clase que la implemente, que tenga un método GetTextToPrint cambiará dependiendo de lo que se quiera imprimir en cada clase.

## Desafío(s)

Este ejemplo es el mismo que hemos utilizado hasta ahora, pero el código tiene modificaciones resultantes de aplicar los principio y patrones anteriores.

La clases que implementan IPrinter, como ConsolePrinter, dependen de la clase Recipe: un mensaje string GetTextToPrint() es enviado a una instancia de Recipe en el método void PrintRecipe(Recipe).

➡️ **Apliquen el principio de inversión de dependencia para que la clase ConsolePrinter no dependa de la clase Recipe.**
