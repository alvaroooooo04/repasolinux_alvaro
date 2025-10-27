# Ejercicios Linux- capítulo 2

[TOC]

## Comandos utilizados

- `cd`

- `pwd`

- `ls`

- `mkdir`

  ![image-20250924100827327](C:\Users\ALUMNO\AppData\Roaming\Typora\typora-user-images\image-20250924100827327.png)

## Ejercicios

1. ¿En qué directorio se encuentran los ficheros de configuración del sistema?

   Están en el directorio `/etc.` 

   ![image-20250924101332421](C:\Users\ALUMNO\AppData\Roaming\Typora\typora-user-images\image-20250924101332421.png)

2. Para entrar en un sistema Linux hace falta a) nombre de usuario, contraseña y dirección IP, b) nombre de usuario y contraseña o c) únicamente una contraseña..

   Nombre de usuario y contraseña.

3.  Muestra el contenido del directorio actual.

​      

```bash
 ls
```

![image-20250924102031484](C:\Users\ALUMNO\AppData\Roaming\Typora\typora-user-images\image-20250924102031484.png)

4. Muestra el contenido del directorio que está justo a un nivel superior

ls.. ![image-20250924102147776](C:\Users\ALUMNO\AppData\Roaming\Typora\typora-user-images\image-20250924102147776.png)

5.  ¿En qué día de la semana naciste?, utiliza la instrucción cal para averiguarlo.

Viernes 24 ![image-20250924102534040](C:\Users\ALUMNO\AppData\Roaming\Typora\typora-user-images\image-20250924102534040.png)






<div style="page-break-after: always;"></div>

6. Muestra los archivos del directorio /bin

   ```bash
   ls /bin
   ```

   

![image-20250924102729018](C:\Users\ALUMNO\AppData\Roaming\Typora\typora-user-images\image-20250924102729018.png)




<div style="page-break-after: always;"></div>

7. Suponiendo que te encuentras en tu directorio personal (/home/nombre), muestra un listado del contenido de /usr/bin a) con una sola línea de comando, b) moviéndote paso a paso por los directorios y c) con dos líneas de comandos.

   a)

   ```bash
   ls /usr/bin
   ```

   ![image-20250924103101793](C:\Users\ALUMNO\AppData\Roaming\Typora\typora-user-images\image-20250924103101793.png)
<div style="page-break-after: always;"></div>

b)

```bash
cd .. 
cd .. 
cd usr 
cd bin 
ls
```

![image-20250924103543389](C:\Users\ALUMNO\AppData\Roaming\Typora\typora-user-images\image-20250924103543389.png)


<div style="page-break-after: always;"></div>

c) 

```bash
cd /usr/bin ls
```

![image-20250924103631772](C:\Users\ALUMNO\AppData\Roaming\Typora\typora-user-images\image-20250924103631772.png)


<div style="page-break-after: always;"></div>

8. Muestra todos los archivos que hay en /etc y todos los que hay dentro de cada subdirectorio, de forma recursiva (con un solo comando).

   ```bash
   ls -R /etc
   ```

   

![image-20250924104044049](C:\Users\ALUMNO\AppData\Roaming\Typora\typora-user-images\image-20250924104044049.png)

9. Muestra todos los archivos del directorio /usr/X11R6/bin ordenados por tamaño (de mayor a menor). Sólo debe aparecer el nombre de cada fichero, sin ninguna otra información adicional.

No existe el directorio ![image-20250924104433975](C:\Users\ALUMNO\AppData\Roaming\Typora\typora-user-images\image-20250924104433975.png)


<div style="page-break-after: always;"></div>



10. Muestra todos los archivos del directorio /etc ordenados por tamaño (de mayor a menor) junto con el resto de características, es decir, permisos, tamaño, fechas de la última modificación, etc. El tamaño de cada fichero debe aparecer en un formato “legible”, o sea, expresado en Kb, Mb, etc.

    ```bash
    ls -Slh /etc
    ```

    ![image-20250924104637403](C:\Users\ALUMNO\AppData\Roaming\Typora\typora-user-images\image-20250924104637403.png) 
<div style="page-break-after: always;"></div>

11. Muestra todos los archivos del directorio /bin ordenados por tamaño (de menor a mayor). Sólo debe aparecer el tamaño y el nombre de cada fichero, sin ninguna otra información adicional. El tamaño de cada fichero debe aparecer en un formato “legible”, o sea, expresado en Kb, Mb, etc.

    ```bash
    ls -Sshr /bin
    ```

    ![image-20250924104835201](C:\Users\ALUMNO\AppData\Roaming\Typora\typora-user-images\image-20250924104835201.png)
<div style="page-break-after: always;"></div>

12. Muestra el contenido del directorio raíz utilizando como argumento de ls una ruta absoluta.

    ```bash
    ls / 
    ```

    ![image-20250924105144879](C:\Users\ALUMNO\AppData\Roaming\Typora\typora-user-images\image-20250924105144879.png)

13. Muestra el contenido del directorio raíz utilizando como argumento de ls una ruta relativa. Suponemos que el directorio actual es /home/elena/documentos.

    ```bash
    ls ../../..
    ```

    ![image-20250924105230503](C:\Users\ALUMNO\AppData\Roaming\Typora\typora-user-images\image-20250924105230503.png)

14. Crea el directorio gastos dentro del directorio personal.

    ```bash
    mkdir gastos
    ```

    , no muestra nada en consola pero se crea.

15. ¿Qué sucede si se intenta crear un directorio dentro de /etc?

    No se puede crear un directorio, al menos un usuario "normal" no puede.

16. Muestra el contenido del fichero /etc/fstab

    ```bash
    cat/etc/fstab
    ```

    ![image-20250924110025500](C:\Users\ALUMNO\AppData\Roaming\Typora\typora-user-images\image-20250924110025500.png)
<div style="page-break-after: always;"></div>

17. Muestra las 10 primeras líneas del fichero /etc/bash.bashrc

```bash
head /etc/bash.bashrc
```

![image-20250924111010867](C:\Users\ALUMNO\AppData\Roaming\Typora\typora-user-images\image-20250924111010867.png)

18.  Crea la siguiente estructura de directorios dentro del directorio de trabajo personal:

```bash
~$ mkdir multimedia 
~$ cd multimedia/
~/multimedia$ mkdir musica imagenes video presentaciones
~/multimedia$ cd imagenes/ 
~/multimedia/imagenes$ mkdir personales otras
```

![image-20250924111427504](C:\Users\ALUMNO\AppData\Roaming\Typora\typora-user-images\image-20250924111427504.png)

19.  Crea un fichero vacío dentro del directorio musica, con nombre estilos_favoritos.txt

```bash
cd multimedia/

cd musica/

touch estilos_favoritos.txt
```

![image-20250924111755480](C:\Users\ALUMNO\AppData\Roaming\Typora\typora-user-images\image-20250924111755480.png)
<div style="page-break-after: always;"></div>

20.Utiliza tu editor preferido para abrir el fichero estilos_favoritos.txt e introduce los estilos de música que más te gusten. Guarda los cambios y sal.

```bash
nano musica/estilos_favoritos.txt
```

![image-20250926104224720](C:\Users\ALUMNO\AppData\Roaming\Typora\typora-user-images\image-20250926104224720.png)

<img src="C:\Users\ALUMNO\AppData\Roaming\Typora\typora-user-images\image-20250926104509724.png" alt="image-20250926104509724" style="zoom:200%;" />

21. Muestra todo el contenido de estilos_favoritos.txt

```bash
cat estilos_favoritos.txt 
```

![image-20250926104617001](C:\Users\ALUMNO\AppData\Roaming\Typora\typora-user-images\image-20250926104617001.png)

22. Muestra las 3 primeras líneas de estilos_favoritos.txt

```bash
head -n 3 estilos_favoritos.txt
```

![image-20250926104757981](C:\Users\ALUMNO\AppData\Roaming\Typora\typora-user-images\image-20250926104757981.png)
<div style="page-break-after: always;"></div>

23. Muestra la última línea de estilos_favoritos.txt

```bash
tail -n 1 estilos_favoritos.txt
```

![image-20250926105017726](C:\Users\ALUMNO\AppData\Roaming\Typora\typora-user-images\image-20250926105017726.png)
<div style="page-break-after: always;"></div>

24. Muestra todo el contenido del fichero estilos_favoritos.txt excepto la primera línea. Se supone que no sabemos de antemano el número de líneas del fichero.

```bash
tail -n +2 estilos_favoritos.txt
```

![image-20250926105124245](C:\Users\ALUMNO\AppData\Roaming\Typora\typora-user-images\image-20250926105124245.png)

Lo muestra así porque la primera línea es vacía.