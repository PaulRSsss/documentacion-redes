DESCRIPCION
Can you crack the password to get the flag?Download the password checker [here](https://artifacts.picoctf.net/c/12/level1.py)
and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/12/level1.flag.txt.enc) in the same directory too.

SOLUCION
picoCTF{545h_r1ng1ng_1b2fd683}
Vi la contraseña directamente del archivo pero igual no me funcionaba, entonces pasé la contraseña al programa usando "printf "8713\n" | python3 level1.py" luego redirigí toda la salida a un archivo con "> salida.bin 2>&1" para capturar todos los caracteres y solicité solo al bandera con el comando "strings salida.bin | grep -i "picoCTF"

NOTAS ADICIONALES
Muy cansado verdaderamente, tuve que investigar varios comandos, ya estuvo suave

REFERENCIAS