# Enunciado didáctico reconstruido — BiometricPrompt + Android Keystore

Laboratorio Android de seguridad destinado a combinar autenticación biométrica y criptografía respaldada por `AndroidKeyStore`.

La aplicación debe:

1. comprobar si el dispositivo puede autenticar mediante biometría fuerte;
2. crear una clave AES no exportable dentro de `AndroidKeyStore`;
3. exigir autenticación para cada uso de la clave;
4. cifrar un texto únicamente tras una autenticación biométrica correcta usando `BiometricPrompt` y `CryptoObject`;
5. almacenar solo el IV y el texto cifrado en almacenamiento privado de la aplicación;
6. realizar una segunda operación biométrica para descifrar el contenido;
7. permitir eliminar tanto la clave como los datos cifrados.

El repositorio es una demostración de API y no pretende implementar un gestor de contraseñas completo.

No existe una base de datos asociada.
