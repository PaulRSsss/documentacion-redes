DESCRIPCION
A veces necesitas gestionar datos de procesos fuera de un archivo. ¿Puedes encontrar una manera de conservar la salida de este programa y buscar la bandera? Conéctate a jupiter.challenges.picoctf.org 4427.
 
SOLUCION
Investigué comandos de búsqueda de filtración ya que me daba una salida muy grande de texto en el que supuse estaría la bandera, utilicé el comando:
ncat jupiter.challenges.picoctf.org 4427 | grep -i "picoCTF"
La solución fue:
picoCTF{digital_plumb3r_5ea1fbd7}

NOTAS ADICIONALES
Muy buen reto

REFERENCIAS