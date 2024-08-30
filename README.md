# RAG local con Python y Flask

Esta aplicación está diseñada para manejar consultas utilizando un modelo de lenguaje y una base de datos vectorial. Genera múltiples versiones de una consulta de usuario para recuperar documentos relevantes y proporciona respuestas basadas en el contexto recuperado.

## Requisitos previos

1. **Python 3**: Asegúrate de tener instalado Python 3.x.
2. **Ollama**: Esta aplicación requiere que Ollama esté instalado y ejecutándose localmente. Sigue la [guía de instalación de Ollama](https://github.com/ollama/ollama/blob/main/README.md#quickstart) para configurarla.

## Configuración

1. **Clonar el repositorio**:
```bash
$ git clone https://github.com/your-repo/local-rag.git
$ cd local-rag
```

2. **Crear un entorno virtual**:
```bash
$ python -m venv venv
$ source venv/bin/activate

# Para usuarios de Windows
# venv\Scripts\activate
```

3. **Instalar dependencias**:
```bash
$ pip install -r requirements.txt
```

4. **Ejecutar Ollama**:
Asegúrese de que Ollama esté instalado y ejecutándose localmente. Consulte la [documentación de Ollama](https://github.com/ollama/ollama/blob/main/README.md#quickstart) para obtener instrucciones de configuración.
- Instalar el modelo llm
```bash
$ ollama pull mistral
```
- Instalar el modelo de incrustación de texto
```bash
$ ollama pull nomic-embed-text
```
- Ejecutar Ollama
```bash
$ ollama serve
```

## Ejecución de la aplicación
```bash
$ python app.py
```

## Conclusión

Esta aplicación aprovecha un modelo de lenguaje y una base de datos de vectores para proporcionar capacidades mejoradas de manejo de consultas. Asegúrese de que Ollama se esté ejecutando localmente y siga las instrucciones de configuración para comenzar.
