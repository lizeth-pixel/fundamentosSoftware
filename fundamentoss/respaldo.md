<div style="display: flex; justify-content: space-between; align-items: center;"><img src="img/logoitt.png"><img src="img/logoitt2.png"></div>

<br>
<br>
<br>
<br>

# <center>**TECNOLÓGICO NACIONAL DE MÉXICO**
## <center>**INSTITUTO TECNOLÓGICO DE MILPA ALTA II**

<br>

### <center>INGENIERIA EN SISTEMAS  COMPUTACIONALES
### <center>SEMESTRE: 5

<br>

### <center>ADMINISTRACIÓN DE BASE DE DATOS
### <center>BOLLAS PAREDES DIEGO ALBERTO

<br>

#### <center><u>**MÉTODOS DE RESPALDO DE UNA BD**</u>

<br>

#### <center> MARTINEZ VELASCO LIZETH
#### <center>NO.C. 241190035

<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>

<p style="text-align: right;">13/noviembre/2026</p>

<br>
<br>
<br>

---

### **INTRODUCCIÓN**

<br>

En esta actividad se comprende qué son los respaldos de bases de datos y por qué son importantes. A veces podemos perder información por error o por algún problema, y tener una copia de seguridad nos ayuda a recuperarla sin perder todo el trabajo. 

<br>
<br>
<br>
<br>
<br>
<br>



---

<br>

### **DESARROLLO**

<br>

### 1. MÉTODOS DE RESPALDO DE UNA BASE DE DATOS

<br>

Un respaldo es hacer una copia de seguridad de toda la información de la base de datos, para poder recuperla si algo pasa.

<br>

##### MÉTODOS PRINCIPALES:

<br>

|**Método**|**¿Qué es?**|**¿Cuándo se usa?**|**Ejemplo**|
|----------|------------|-------------------|-----------|
|**Respaldo Frío**|Se hace con la base de datos apagada. Copias directamente los archivos donde está guardada la información. Es seguro porque nadie está usando la base al momento de copiarla.|Cuando puedes detener el servicio por un rato. Es muy común en horarios de poca actividad.|Apagas MySQL -> copias la carpeta **`prueba`** -> la pegas en tu carpeta de respaldos.|
|**Respaldo Caliente**|Se hace mientras lka base está encendida y en uso. No hay que detener nada. Se usan comandos especiales que no bloquean el trabajo de los usuarios.|Cuando la base se usa todo el dia y no se puede apagar.|Usar el comando **`mysqldumnp`** desde la consola mientras el sistema sigue funcionando.|
|**Respaldo Lógico**|Genera un archivo con instrucciones de texto (código SQL) para volver a crear las tablas y los datos. Es el más fácil de leer y mover entre diferentes equpos.|Para tareas escolares, proyectos pequeños o cuando necesitas restaurar fácilmente.|Exportar la base desde phpMyAdmin o con el comando **`mysqldumnp`** -> obtines unarchivo **`.sql`**.|

<br>

---

<br>

### **CONLUSIÓN**

<br>

Al terminar esta práctica entendí que hacer respaldos no es difícil y que es algo que siempre debemos hacer cuando trabajamos con información importante. Aprendí también la diferencia entre respaldo frío, caliente y lógico, y ahora sé cuál usar según la situación.