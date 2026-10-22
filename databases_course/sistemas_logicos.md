## SISTEMAS LÓGICOS (Logical systems)

Un **Sistema Lógico de almacenamiento** es la forma de organizar la información para guardarla y recuperarla, con independencia del soporte físico donde acabe grabada.

Aprenderemos 4 palabras que vamos a usar durante todo el curso:

1. **Fichero**
2. **Registro Lógico**
3. **Campo**
4. **Clave**

La cantidad de información que se transfiere entre el disco y la memoria en una sola operación de lectura o escritura se llama **registro físico** o **bloque.**Normalmente un bloque contiene varios registros lógicos: al número de registros lógicos que caben en un bloque se le llama **factor de bloque** (o de blocaje), y a la operación de agruparlos, **bloque de registros.**

## TIPOS DE FICHEROS SEGÚN SU CONTENIDO

Según cómo se codifica lo que guardan, hay 2 grandes tipos de ficheros:

1. **Los ficheros de texto plano:** contienen sólo carácteres de una codificación determinada, como ASCII o UTF-8. Una persona entiende su contenido con cualquier editor de texto: **.txt**, **.csv**, **.html**, **.xml****.json**. Aunque no lo parezca, sirven perfectamente para guardar información estructurada: en un **.csv** cada registro ocupa una línea y los campos se separan con comas, puntos y comas tabuladores.

2. **Los ficheros binarios:** contienen información codificada para que la procese un programa concreto. Abiertos con un editor de texto, parecen basura: *.exe*,*.pdg*,*.jpg*,*.mp3*,*.docx* o en los ficheros de datos de un SGBD. La misma información suele ocupar menos en binario que en texto.
