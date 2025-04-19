# Proyecto-de-Final-IA

## Nombre

YEREMMY WILLIAM TRAVIESO PEÑA

## Matrícula

23-EISN-2-071

## Proyecto

# Generador de Pokémon por Tipo

## Descripción

Este proyecto es una aplicación interactiva que utiliza inteligencia artificial para generar un Pokémon ficticio según el tipo que el usuario seleccione o diga por voz. La aplicación usa modelos avanzados de lenguaje para crear una descripción del Pokémon, genera una imagen única utilizando DALL·E 3, y convierte esa descripción en una narración por voz para crear una experiencia completa e inmersiva.

## Características principales

- **Generación de descripción**: Utiliza OpenAI GPT-3.5-Turbo para crear una breve historia o descripción de un Pokémon ficticio según su tipo.
- **Imágenes generadas con IA**: Usa DALL·E 3 para generar una imagen visual del Pokémon inventado.
- **Narración por voz**: Convierte el texto generado a voz en español utilizando gTTS.
- **Reconocimiento de voz**: Permite que el usuario diga por micrófono el tipo de Pokémon que desea generar.
- **Interfaz amigable**: Diseñada con Gradio para facilitar la interacción del usuario sin necesidad de código.

## Tecnologías utilizadas

- **Python 3.10+**
- **Gradio**: Para la interfaz gráfica del usuario
- **OpenAI API**:
  - GPT-3.5-Turbo para la generación de texto
  - DALL·E 3 para la generación de imágenes
- **gTTS**: Síntesis de voz en español
- **SpeechRecognition**: Para capturar comandos de voz del usuario

## Estructura del proyecto

```
├── app.py               # Aplicación principal con Gradio
├── requirements.txt     # Librerías necesarias para ejecutar el proyecto
├── README.md            # Descripción del proyecto
```

## Instalación

### Requisitos previos

- Python 3.10 o superior
- Cuenta en OpenAI con una API key válida

### Pasos para la instalación

1. Clona este repositorio:
   ```bash
   git clone https://github.com/Box-48/Proyecto-Final-IA.git
   cd Proyecto-Final-IA
   ```

2. Instala las dependencias:
   ```bash
   pip install -r requirements.txt
   ```

3. Agrega tu clave API:
   Abre `app.py` y coloca tu API key de OpenAI donde se indica:
   ```python
   client = OpenAI(api_key="sk-tu-api-key-aqui")
   ```

## Uso

1. Ejecuta la aplicación:
   ```bash
   python app.py
   ```

2. Abre el enlace `http://127.0.0.1:7860` que aparecerá en la terminal.

3. En la interfaz, puedes:
   - Seleccionar un tipo de Pokémon del menú desplegable
   - O grabar tu voz diciendo el tipo (por ejemplo: “planta”, “dragón”, etc.)

4. La aplicación generará:
   - Una imagen ilustrativa del Pokémon con DALL·E 3
   - Una descripción con GPT-3.5-Turbo
   - Y una narración con voz automática (gTTS)

## Flujo de trabajo interno

1. El usuario selecciona o dice un tipo de Pokémon.
2. GPT-3.5 genera una descripción de un Pokémon ficticio del tipo indicado.
3. DALL·E 3 genera una imagen a partir del prompt construido.
4. gTTS convierte la descripción en audio.
5. La interfaz muestra la imagen, la descripción y reproduce la voz.

## Personalización

- Puedes ajustar los prompts en la función `prompt_imagen()` para cambiar el estilo visual.
- Puedes modificar la voz o idioma de gTTS en la función `texto_a_audio()`.
- También puedes adaptar los tipos válidos modificando la lista `pokemon_types`.

## Notas importantes

- La aplicación requiere conexión a internet para acceder a la API de OpenAI.
- Asegúrate de tener saldo o cuota activa en tu cuenta de OpenAI.
- Las imágenes generadas pueden tardar unos segundos, especialmente en tamaño `1024x1024`.

## Contribuciones

¡Las contribuciones son bienvenidas! Si deseas mejorar el proyecto:

1. Haz un fork del repositorio
2. Crea una rama nueva (`git checkout -b mejora-x`)
3. Realiza tus cambios y haz commit
4. Sube tu rama (`git push origin mejora-x`)
5. Abre un Pull Request en GitHub

## Contacto

YEREMMY WILLIAM TRAVIESO PEÑA  
Matrícula: 23-EISN-2-071

Enlace del proyecto: [https://github.com/Box-48/Proyecto-Final-IA](https://github.com/Box-48/Proyecto-Final-IA)
