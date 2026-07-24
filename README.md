# Prompt Studio · Clase 2

Herramienta interactiva de apoyo para **Prompting Avanzado**. Replica el patrón pedagógico de `ayudas-tecnicas/prompt-lab/` —práctica individual más tablero docente— sin repetir el ejercicio de etiquetar Acción, Contexto y Modificadores.

## Qué practica

La experiencia tiene ocho misiones:

1. Completar una estructura profesional.
2. Elegir cuándo usar few-shot.
3. Hacer explícito el criterio de análisis.
4. Ordenar una cadena de prompts.
5. Escoger un buen ejemplo entrada → salida.
6. Organizar información con etiquetas.
7. Refinar una respuesta con instrucciones precisas.
8. Detectar señales de alerta en una salida de IA.

Las misiones se agrupan en cinco competencias que aparecen en el tablero:

- Estructura profesional
- Selección de técnica
- Prompt chaining
- Organización y control
- Evaluación crítica

## Archivos

```text
prompt-studio/
├── estudiante.html  # experiencia móvil/desktop para el grupo
├── profesor.html    # tablero en vivo para proyectar
└── README.md
```

## Cómo usarlo

Desde la raíz del repositorio:

```powershell
python -m http.server 8080
```

Abrir:

- Estudiantes: `http://localhost:8080/docs/slides/clase-2-prompting-avanzado/prompt-studio/estudiante.html`
- Profesor: `http://localhost:8080/docs/slides/clase-2-prompting-avanzado/prompt-studio/profesor.html`

Para una clase real, ambos archivos deben estar publicados por HTTP/HTTPS. El flujo está preparado para GitHub Pages si se publica este repositorio.

## Datos en tiempo real

Usa el mismo proyecto Firebase de Prompt Lab, pero guarda los datos en una ruta independiente:

```text
/prompt_studio_clase2/
```

El botón **Reiniciar sesión** del tablero solo elimina esa ruta; no toca los resultados de Clase 1.

La vista de estudiante sigue funcionando si Firebase no carga, pero en ese caso el resultado se conserva únicamente en la sesión del navegador y no aparecerá en el tablero.

## Flujo recomendado en clase

- Instructor: abre y proyecta `profesor.html`.
- Grupo: abre `estudiante.html`, escribe su nombre y completa las ocho misiones.
- Instructor: observa la precisión por misión y el mapa de habilidades.
- Debrief: empieza por la misión con menor promedio y pide a dos personas que expliquen su criterio antes de revelar la respuesta.

Tiempo estimado: **8–10 minutos de práctica + 5 minutos de conversación**.
