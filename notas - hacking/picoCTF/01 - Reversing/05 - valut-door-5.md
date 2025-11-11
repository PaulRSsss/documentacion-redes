DESCRIPCION
In the last challenge, you mastered octal (base 8), decimal (base 10), and hexadecimal (base 16) numbers, but this vault door uses a different change of base as well as URL encoding!The source code for this vault is here: [VaultDoor5.java](https://challenge-files.picoctf.net/c_fickle_tempest/aee691634d8cfd4a10820634bdea6b80aa104301e4b83d01fd4d176098d69e99/VaultDoor5.java)

SOLUCION
Decodifiqué el `expected` de Base64 a la cadena con `%xx`, y luego apliqué URL-decode para obtener el texto original
picoCTF{c0nv3rt1ng_fr0m_ba5e_64_ed0b4288}

NOTAS ADICIONALES
Entretenido

REFERENCIAS