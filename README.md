# bianca_db

Este repositorio sirve para agregar los cambios al esquema de base de datos Bianca.

## Buenas prácticas

- Los archivos de migración deben tener un nombre correlativo (por ejemplo, `0001_bianca.sql`, `0002_bianca.sql`).
- Cada archivo no debe superar las 1000 líneas.
- Crea siempre una nueva rama `feature/` o `fix/` o `bug/` para nuevos cambios.
- Documenta cada segmento de código con un comentario descriptivo antecedido por el número de PR (ejemplo, `# PR-12 se agrega columna estado para conocer si el registro se encuentra activo o inactivo`).
- Realiza revisiones de código antes de fusionar cambios a la rama principal.
- Corre los unit tests antes de fusionar cambios a la rama principal
- Aplica cambios a los esquemas en los diferentes entornos (manual o con Github CI) al aceptar el PR.
- No eliminar tablas directamente, en su lugar renombrarlas con un subfijo `_DELETE_ME`
- No eliminar columnas directamente, en su lugar renombrarlas con un subfijo `_DELETE_ME`
