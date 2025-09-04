DESCRIPCION
Can you find the flag in [file](https://jupiter.challenges.picoctf.org/static/94d00153b0057d37da225ee79a846c62/strings) without running it?
 
SOLUCION
usé estos comandos:
cd "/c/Users/$USERNAME/Downloads"
ls -lh
f=strings
ls -lh "$f"
sha256sum "$f"
file "$f" ---aquí me dijo que era arcihvo ELF de linux
xxd -l 64 -g 1 "$f" --- aquí lo confirmé

$string -n 4 "$f" | grep -niE 'flag\{|flag|ctf|key|token|pass' | head -n 30 --- 
busqué dentro del ejecutable todas las cadenas de 4 o más carácteres, con group niE apliqué que me diera solo las palabras que coincidieran con "flag, ctf, key, token, pass" y con head -n 30 solo las primeras 30, pero en todo ese texto manualmente encontré la bandera, aún asi quise encontrar el como hacerlo con comandos y lo resolví con esto:
$strings "$f" | grep -oE 'picoCTF\{[^}]+\}'
y la solución fue:

picoCTF{5tRIng5_1T_d66c7bb7}

NOTAS ADICIONALES
excelente reto que me impulsó 

REFERENCIAS