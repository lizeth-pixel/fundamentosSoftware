# EXAMEN UNIDAD 4 - TIPO B

**Nombre:** `Martinez Velasco Lizeth`
**Grupo:** `5SIS`
**Carrera:** `Ingenieria en Sistemas Computacionales` 
**Fecha:** `10/11/2026`
**Docente:** `Ing. Diego Alberto Bollas Paredes`

---

**Instrucciones:**
- Responde con claridad y justifica tus respuestas. No se evaluarán únicamente definiciones memorizadas.
- Da formato a cada una de tus respuestas.

---

**1. ¿En qué consiste una inyección de código SQL?**

*Respuesta: Son acciones maliciosas que pueden hacer en la base de datos, como eliminar, actualizar, crear o insertar datos en sentencias SQL.*

---

**2. Identifica si existe algún error en la siguiente línea de código y escribe la corrección pertinente y describe tu solución, en caso de no detectar algún error, describe la razón.**
```php
$host = "maridb:host=".hostname.";dbname=".$db_name;
```

*Respuesta: 
```php
"mariadb:host= $user, $password, $dbname;.hostname;";*
```

---

**3. ¿Qué es phpMyAdmin?**

*Respuesta: Es una herramienta web gratuita, desarrollada por PHP, sirve como administrador de base de datos de MySQL y MariaDB mediante una interfaz gráfica.*

---

**4. ¿Para que sirve el argumento PDO::FETCH_ASSOC en una función fetch?**

*Respuesta: Para obtener un valor asociado.*

---

**5. ¿Qué es una consulta blinda?**

*Respuesta: Protege las insatrucciones SQL *

---

**6. Escribe una función en `PHP` que permita insertar tres datos `nombre`,`apellido`,`edad` a una tabla `t_persona.` Documenta cada parte que la conforma.**

*Respuesta: 
```php
function insercion($conexion, $nombre, $apellido, $edad){
    echo "<h1>Insercion</h1>";
    $query = "INSERT INTO t_persona ('$nombre', '$apellido', '$edad')";
    $conexion -> exec($query);
    "<br>";
    echo "Inserción finalizada (".$nombre.", ".$apellido.", ".$edad.")";
    "<br>";
}
insercion($conexion, "examen")
```
*

---

**7. Escribe y señala cada parte del código correspondiente para crear una *conexión a Base de Datos* con `PHP` y `PDO`.**

*Respuesta:

```php
<?
$hostname = localhost
$user = liz
$password = liz123
$dbname = examen

try {
    PDO
}
>
```
*

---

**8. Describe cada línea del siguiente código:**
```php
function eliminacion($conexion, $nombre){
    echo "<h1>Eliminacion</h1>";
    $query = "DELETE FROM t_cliente WHERE nombre= '$nombre' ";
    $conexion -> exec($query);
    "<br>";
    echo "Eliminación finalizada (".$nombre.")";
    "<br>";
}
eliminacion($conexion, "examen");
```
*Respuesta: es una función de eliminación el cual tiene un query que funciona para la instruccion de DELETE y el exec se encarga de hacer funcionar la instruccion SQL*

---

**9. ¿Qué es apache?**

*Respuesta: Es el servidor web para de un sistema gestor de base de datos.*

---

**10. ¿Qué son los Binary log?**

*Respuesta: Son los que almacena o actualizan los errores de un servidor de una base de datos.*