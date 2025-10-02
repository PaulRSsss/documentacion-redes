DESCRIPCION
Can you crack the password to get the flag?Download the password checker [here](https://artifacts.picoctf.net/c/14/level2.py)and you'll need the encrypted [flag](https://artifacts.picoctf.net/c/14/level2.flag.txt.enc) in the same directory too.

SOLUCION
picoCTF{tr45h_51ng1ng_9701e681}
Parecido al anterior, utilicé $ grep -n '(aquí va otro = pero se pone todo amarillo)=' level2.py || sed -n '2,120p' level1.py para buscar la contraseña al definirse con == o las primeras 120 lineas en su defecto, me lo dio en hexadecimal y al traducirlo usé ""$ printf "4ec9\n" | python3 level2.py > salida.bin 2>&1""  para ejecutar ya con la contraseña el archivo y guardar la contraseña en automático, por último aplico el comando ""strings salida.bin | grep -i "picoCTF" || true"" para tomar ese mismo archivo creado y filtrar hasta encontrar picoCTF 

NOTAS ADICIONALES
Estoy cansado profe

REFERENCIAS