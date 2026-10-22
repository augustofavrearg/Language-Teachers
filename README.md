# Language-Teachers

Colección de skills para aprender y enseñar idiomas con tutores personales de IA. Cada persona puede descargar un tutor, personalizarlo para su uso y crear un puente entre el idioma que conoce y el que quiere aprender.

## Tutores disponibles

| Carpeta | Identificador del skill | Idioma que enseña | Idioma de apoyo |
|---|---|---|---|
| [English-Teacher](English-Teacher/README.md) | `english-teacher` | Inglés | Español |

English-Teacher incluye clases breves, correcciones, gramática por capas y juegos. Su recorrido predeterminado va de A1 a A2, con orientación para adaptar las clases a A1–C2.

## Descargar e instalar un tutor

```bash
git clone https://github.com/augustofavrearg/Language-Teachers.git
```

También puedes descargar el ZIP desde GitHub. Para instalar English-Teacher en Codex, copia el contenido de `English-Teacher/` a una carpeta llamada `english-teacher` dentro de tu directorio de skills, habitualmente `~/.codex/skills/` o `$CODEX_HOME/skills/` si lo configuraste. Conserva una copia de cualquier versión personalizada antes de reemplazarla e inicia una nueva sesión después de instalar.

La carpeta del repositorio usa `English-Teacher`; la carpeta instalada y el campo `name` del skill usan `english-teacher`.

```text
Usa $english-teacher. Hablo español y quiero aprender inglés desde A1.
Dame una explicación breve y un ejercicio por turno.
```

## Crear tu propio tutor o puente entre idiomas

Puedes modificar tu copia para uso personal o hacer un fork y compartir un nuevo tutor. No hace falta contribuir al repositorio para personalizar un skill.

1. Copia `English-Teacher/` a una carpeta descriptiva, como `French-From-Spanish/`.
2. Cambia el `name` de `SKILL.md` a un identificador en minúsculas con guiones, como `french-from-spanish`. Ajusta también su `description` para indicar qué enseña y cuándo usarlo.
3. Define el idioma de origen o apoyo y el idioma objetivo. Por ejemplo: español → francés. Para un puente en ambos sentidos, explica cuándo practicar cada dirección.
4. Adapta las instrucciones, los ejemplos, los juegos, las correcciones y los archivos de `references/`. Revisa las reglas propias del inglés; una traducción literal no basta.
5. Actualiza `agents/openai.yaml` y el README del tutor con el nuevo nombre, propósito y ejemplos de invocación.
6. Instálalo en una carpeta que coincida con su `name` y prueba una clase, una corrección y un ejercicio en cada dirección que ofrezca.

Un tutor debe aclarar el nivel inicial, los objetivos, el idioma de las explicaciones y cómo dará feedback. El idioma de apoyo y el idioma objetivo se configuran en sus instrucciones; el repositorio no implementa un sistema automático de comunicación entre skills.

Para compartir cambios, consulta [CONTRIBUTING.md](CONTRIBUTING.md).

## Estructura

```text
Language-Teachers/
├── README.md
├── CONTRIBUTING.md
├── LICENSE
└── English-Teacher/
    ├── README.md
    ├── SKILL.md
    ├── agents/openai.yaml
    └── references/
        ├── cefr-path.md
        └── grammar-layers.md
```

## Licencia

[MIT](LICENSE): puedes usar, modificar y compartir los tutores, conservando el aviso de copyright y la licencia.
