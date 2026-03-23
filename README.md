Restricciones XML mediante REGEX y XSD
1.Restricción de nombre 
  "[A-Za-zÁÉÍÓÚáéíóúñÑ\s]+" 
Ésta restricción permite todos los caracteres , mayúsculas y minúsculas desde a la letra A a la letra Z. Igualmente permite las vocales con acento , la ñ y Ñ y espacios por si se tiene nombre compuesto

2. Restricción de apellidos
  "[A-Za-zÁÉÍÓÚáéíóúñÑ\s]+"
Igual que el nombre, hace lo mismo

3.Restricción de email
  "\S+@\S+\.\S+"
Permite cualquier numero de carácteres , un arroba , cualquier número de carácteres , un . y cualquier numero de carácteres. 

4. Restricción de teléfono
   "([0-9]{3}[\s][0-9]{3}[\s][0-9]{3})?([0-9]{9})?"
Valida cualquier teléfono puesto de 3 en 3 hasta 9 o nueve números seguidos

5.Restricción de dirección
  "[A-Za-zÁÉÍÓÚáéíóúñÑ\s0-9,.-]+"
Igual que el nombre y los apellidos pero le he añadido para que pueda poner numeros , la contrabarra , la coma punto y guión

6.Restricción de códigoPostal
  "[0-9]{5}"
Sencillamente permite 5 números

7.Restricción de nombreUsuario
  [A-Za-zÁÉÍÓÚáéíóúñÑ]+
He usado el mismo que los nombres pero no he permitido los espacios.

8.Restricción de contraseña
  "[a-zA-Z0-9@#_.\-]+"
He permitido una contaseña de min 8 de longitud y max 15 pero con los carácteres que he permitido arriba 

9.Restricción de fecha nacimiento
En este campo he permitido cualquier fecha pero acortando a un rango prudente como se puede observar en el XSD
