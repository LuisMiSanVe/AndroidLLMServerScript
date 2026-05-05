> [Ver en ingles/See in english](https://github.com/LuisMiSanVe/AndroidLLMServerScript/blob/main/README.md)
# 📲 Script para Servidor de LLMs en Android
[![image](https://img.shields.io/badge/json-5E5C5C?style=for-the-badge&logo=json&logoColor=white)](https://www.newtonsoft.com/json)
[![image](https://img.shields.io/badge/Visual_Studio_Code-0078D4?style=for-the-badge&logo=visual%20studio%20code&logoColor=white)](https://code.visualstudio.com/)
[![image](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)](https://developer.android.com/studio)
[![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)](https://www.python.org/)
[![JS](https://img.shields.io/badge/javascript-%23ff8040.svg?style=for-the-badge&logo=JavaScript&logoColor=ffffff)](https://developer.mozilla.org/docs/Web/JavaScript)


Script de Python que levanta un servidor Localhost de LLMs usando [llama.cpp](https://github.com/ggml-org/llama.cpp) en Android.

## 📝 Explicación de Tecnología
Este script te permite crear un Servicio de LLMs usando un dispositivo Android como servidor.

`Termux` de Android no es capaz de compilar `llama-server` debido a la falta de librerías necesarias, este script de python hace un arreglo al usar `llama-simple` en su lugar.

## 🛠️ Instalación
En tu dispositivo Android 13+ (probado), instala Termux y ejecuta los siguientes comandos:

```
pkg update && pkg upgrade
pkg install git cmake clang wget python
```

Entonces clona e instala `llama.cpp` siguiendo su guia.

Consigue un modelo LLM relativo a tu dispositivo.

Entonces, adapta el script de Python a tu estructura de carpetas y copialo a tu dispositivo Android, y ejecutalo:

```
python server.py
```

Así, tu servicio estaría publicado en tu red local y se quedará escuchando en el puerto `8000` por defecto.

## ⚙️ Explicación de uso del proyecto
Para probar el servicio, puedes usar la web HTML cliente `test.html`, esta además incluye diversas opciones y ajustes para probar tu LLM local.

## 💻 Tecnologías usadas
- Lenguaje de programación: [Python](https://www.python.org/), [JavaScript](https://developer.mozilla.org/docs/Web/JavaScript)
- Probado en: [Android 13 (MAUI)](https://www.android.com/)
- Librerías: [urllib](https://docs.python.org/es/3/library/urllib.html)
- Otros:
    - [llama.cpp](https://github.com/ggml-org/llama.cpp)
    - [Termux](https://f-droid.org/es/packages/com.termux/)
- IDE Recomendado: [VS Code](https://code.visualstudio.com/)
