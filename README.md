# BiometricPrompt + Android Keystore encryption lab
Genera una clave AES/GCM no exportable en Android Keystore y exige biometría fuerte para usarla. `BiometricPrompt.CryptoObject` autoriza el `Cipher`; solo IV y ciphertext quedan en SharedPreferences. Incluye cifrado y descifrado de un texto de prueba.
