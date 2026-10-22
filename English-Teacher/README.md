# English Teacher

Skill para aprender inglés con un tutor personal: explicaciones breves, práctica guiada y correcciones con apoyo en español. El recorrido predeterminado va de A1 a A2, con orientación para adaptar las clases a niveles A1–C2 del MCER.

## Qué incluye

- Clases y planes de estudio adaptados al nivel del estudiante.
- Gramática por capas: verbo, tiempo, aspecto, voz, modalidad, negación y preguntas.
- Práctica de conversación, lectura, construcción y análisis de oraciones.
- Juegos como `Sentence Classifier`, `Aspect Triad`, `Be Three Ways` y `Story Detective`.

## Instalación manual en Codex

Descarga el repositorio Language-Teachers y copia el contenido de `English-Teacher/` a la carpeta `english-teacher` dentro de tu directorio de skills de Codex (habitualmente `~/.codex/skills/`):

```text
english-teacher/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── cefr-path.md
    └── grammar-layers.md
```

Si configuraste `CODEX_HOME`, utiliza su subdirectorio `skills/`. Conserva cualquier versión local que hayas personalizado antes de reemplazar archivos. Inicia una nueva sesión de Codex después de instalarlo.

## Cómo usarlo

Pide una clase indicando el skill, tu nivel y tu objetivo:

```text
Usa $english-teacher. Mi nivel es A1 y quiero avanzar hacia A2.
Explica en español y usa ejemplos en inglés.
Comencemos con una clase corta sobre present simple.
```

También puedes pedir actividades concretas:

```text
Usa $english-teacher para practicar una conversación en un restaurante.
```

```text
Usa $english-teacher y analiza por capas: I have been studying English.
```

Con el skill activo, escribe `&play` para ver las categorías de juegos, o inicia uno directamente:

```text
&play/classification/sentence-classifier
&play/triads/aspect-triad
&play/be-practice/be-three-ways
&play/reading/story-detective
```

Estos comandos son convenciones de conversación interpretadas por el tutor.

## Archivos

`SKILL.md` contiene las instrucciones del tutor; `agents/openai.yaml`, los metadatos de interfaz; y `references/`, las guías de niveles y gramática. El skill funciona mediante instrucciones y no requiere scripts ni servicios externos.
