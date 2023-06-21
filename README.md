<h1>Criptografía Práctica y Blockchain</h1>
<h2>Trabajo Práctico 2</h2>
<h3>Consigna</h3>
<p>Las pruebas de validez nos permiten probar que un cómputo se ha realizado
correctamente en un tiempo bastante menor que la verificación trivial, es decir, que el
cómputo sea corrido de manera independiente por el verificador. En este trabajo
práctico, nos enfocaremos en el sistema de pruebas STARKs en forma simplificada.
Para el trabajo práctico, se podrá hacer uso de las herramientas provistas en
https://github.com/starkware-industries/stark101 (python) o
https://github.com/lambdaclass/STARK101-rs/tree/main (rust).
<br><br>
El objetivo consiste en probar la validez de un programa que calcula 2^{8^20} módulo
p, utilizando diferentes estrategias y viendo el perfil de costos (tanto en términos de
longitud de la prueba como de tiempo de generación). Las estrategias propuestas son:
<br>
1. Considerar a_0 = 2 y a_{n+1}=a_n^8.
<br>
2. Considerar a_0 = 2 y a_{n+1}=a_n^2
<br>
3. Considerar a_0 = 2 y a_{2n+1}=a_{2n}^2 y a_{2n}=a_{2n-1}^4.
<br>
4. Usando 2 columnas.
<br><br>
Tener en cuenta que, dado el grado de las restricciones, se requiere usar un factor de
expansión (blowup) por lo menos tan grande como el grado de las restricciones.</p>
