## SISTEMAS LÓGICOS (Logical systems)

Un **Sistema Lógico de almacenamiento** es la forma de organizar la información para guardarla y recuperarla,  con independencia del soporte físico donde acabe grabada.

Aprenderemos 4 palabras que vamos a usar durante todo el curso:

1. **Fichero**
2. **Registro Lógico**
3. **Campo**
4. **Clave**

La cantidad de información que se transfiere entre el disco y la memoria en una sola operación de lectura o escritura se llama **registro físico** o **bloque.**Normalmente un bloque contiene varios registros lógicos: al número de registros lógicos que caben en un bloque se le llama **factor de bloque** (o de blocaje), y a la operación de agruparlos, **bloque de registros.**

## TIPOS DE FICHEROS SEGÚN SU CONTENIDO

Según cómo se codifica lo que guardan, hay 2 grandes tipos de ficheros:

1. **Los ficheros de texto plano:** contienen sólo carácteres de una codificación determinada, como ASCII o UTF-8. Una persona entiende su contenido con cualquier editor de texto: **.txt**, **.csv**, **.html**, **.xml**,**.json**. Aunque no lo parezca, sirven perfectamente para guardar información estructurada: en un **.csv** cada registro ocupa una línea y los campos se separan con comas, puntos y comas tabuladores.

2. **Los ficheros binarios:** contienen información codificada para que la procese un programa concreto. Abiertos con un editor de texto, parecen basura: **.exe**, **.pdg**, **.jpg**, **.mp3**, **.docx** o en los ficheros de datos de un SGBD. La misma información suele ocupar menos en binario que en texto.

## TIPOS DE FICHEROS SEGÚN SU FUNCIÓN

### FICHEROS PERMANENTES
Contienen los datos que necesita la aplicación para funcionar y duran mucho tiempo. Los **maestos** guardan el estado actual de los datos principales y se modifican a menudo; son el núcleo de la aplicación. Los **constantes** tienen datos que casi nunca cambian y se usan sobre todo para consultar. Los **históricos** guardan datos que fueron actuales en el pasado y sirven para reconstruir situaciones o hacer estadísticas.

### FICHEROS TEMPORALES
Los ficheros temporales se generan a partir de los permanentes para una tarea concreta y desaparecen al terminarla. Los **intermedios** pasan resultados de un programa a otro; los **de maniobras** guardan datos que no caben en la memoria principal mientras se procesan (por ejemplo, al ordenar un fichero enorme); y los **de resultados** contienen datos listos para enviarse a un dispositivo de salida, como una impresora.

## LOS SOPORTES DE ALMACENAMIENTO

Los ficheros se graban en soportes que manejan dispositivos periféricos. Según cómo se llega a los datos, hay 2 tipos:

### SOPORTES SECUENCIALES
1. **Como se accede:** Para leer un dato hay que pasar por todos los anteriores.
2. **Ejemplos:** Cintas magnéticas.
3. **Organizaciones posibles:** solo secuancial.
4. **Uso actual:** copias de seguridad y archivo a largo plazo.

### SOPORTES DIRECCIONALES
1. **Como se accede:** Se puede ir directamente a una posición sin recorrer lo que hay antes.
2. **Ejemplos:** Discos duros, unidades de estado sólido, memorias USB.
3. **Organizaciones posibles:** Secuencial, directa, indexada y cualquier otra.
4. **Uso actual:** todo lo demás.

[**Link de una mejor explicación**](https://academy-code.codingia.com/tipos-de-soportes-de-almacenamiento-y-su-gestion-en-los-sistemas-operativos/#:~:text=En%20los%20soportes%20secuenciales%2C%20los%20datos%20se%20graban,cl%C3%A1sico%20de%20soporte%20secuencial%20es%20la%20cinta%20magn%C3%A9tica.)