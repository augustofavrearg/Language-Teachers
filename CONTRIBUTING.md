# Contribuir a Language-Teachers

Puedes proponer mejoras o un nuevo tutor mediante una pull request. Para uso personal, basta con modificar tu copia local.

## Nuevo tutor

Crea una carpeta con un nombre claro que indique el idioma objetivo y, cuando sea relevante, el idioma de origen: por ejemplo, `French-From-Spanish/`. Utiliza un identificador único en minúsculas y con guiones en el campo `name` de `SKILL.md`.

Incluye:

- `SKILL.md` con `name`, `description` e instrucciones completas para el tutor.
- Un README que indique idiomas de origen y objetivo, nivel inicial, instalación y ejemplos.
- Referencias solo cuando aporten orientación necesaria para ese tutor.
- Metadatos de `agents/openai.yaml` coherentes si incluyes ese archivo.

Adapta la pedagogía al idioma. Revisa ejemplos y correcciones con atención a las diferencias entre ambos idiomas. Si el tutor enseña en ambas direcciones, prueba cada dirección.

Añade el tutor a la tabla del README principal y comprueba que los enlaces relativos funcionan. Explica en la pull request qué enseña y qué ejemplos usaste para comprobar su comportamiento.

No incluyas conversaciones personales, datos de estudiantes, credenciales ni exportaciones generadas. Comparte únicamente material propio o que tengas permiso para redistribuir bajo la licencia del proyecto.
