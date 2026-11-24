# INSTALACIÓN Y CONFIGURACIÓN DE MariaDB

Antes de instalar **`MariaDB`** se hace lo siguiente:
##### 1. Actualizar indices de paquetes:
```bash
sudo apt update
```
---
### Comenzar la instalación de **`MariaDB`**:

##### 1. Instalar el servidor y el cliente:
```bash
sudo apt install mariadb-server mariadb-client -y
```
##### 2. Habilitar el servicio para que inicie el sistema:
```bash
sudo systemctl enable mariadb
```
##### 3. Iniciar el servicio:
```bash
sudo systemctl start mariadb
```
- Detener: stop
- Reiniciar: restart
##### 4. Verificar el estado del servicio:
```bash
sudo systemctl status mariadb
```
##### 5. Ejecutar el script de aseguramiento inicial:
```bash 
sudo mariadb-secure-installation
```
---
-  **`NOTA`**: 
**mariadb-secure-installation** solicita:      
    - Definir contraseña de root
    - Eliminar usuarios anonimos 
    - Deshabilitar el login remoto de root 
    - Eliminar bases de datos 'test' y recargar los privilegios

    ***Todas estas respuestas deben ser 'Y'(sí).***


