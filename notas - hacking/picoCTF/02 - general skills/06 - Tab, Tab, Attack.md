DESCRIPCION
Hay un script interesante en el directorio personal del usuario.
El ordenador del trabajo está ejecutando SSH. Nos han proporcionado un script que realiza algunos cálculos básicos. Explóralo y encuentra una bandera

SOLUCION
Descargué la carpeta e ingresé desde git bash a la ubicación, luego hice un ls -la, y después apliqué el comando ""$ grep -R "picoCTF{" . 2>/dev/null"" pero se negaba a dármelo porque era binario, entonces lo forcé con ""$ grep -aR "picoCTF{" . 2>/dev/null"" y obtuve un texto en el que estaba la llave:
picoCTF{l3v3l_up!_t4k3_4_r35t!_a00cae70}

NOTAS ADICIONALES
Buen reto, bastante complicados

REFERENCIAS