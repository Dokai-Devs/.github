# Cómo trabajamos en Dokai-Devs

Vale para todos los repos de la organización: los de práctica, las plantillas y los de clientes. Nada llega a `main` sin un PR revisado.

## El flujo

1. **Issue.** Descripción, criterios de aceptación y responsable. Usá las plantillas "Tarea" o "Entrega de formación".
2. **Rama corta** con el número del issue: `feat/12-formulario`, `fix/15-fecha-mal`.
3. **PR** completando la plantilla: qué cambia, cómo lo probaste y capturas si toca pantallas. CI tiene que estar en verde.
4. **Revisión.** Los comentarios se responden en el PR. Cada comentario explica el porqué.
5. **Preview de Vercel**, si el repo tiene uno, para probar el cambio antes de mergear.
6. **Merge a `main`** con "Squash and merge". La rama se borra sola.

## Reglas que no se negocian

- No se mergea código que no puedas explicar, probar y mantener, aunque lo haya escrito una IA.
- Las claves viven en Vercel o en el gestor de contraseñas. Nunca en el repo ni en el chat.
- El esquema de la base cambia solo con migraciones.
- Toda tabla con datos de usuarios tiene RLS y un test que lo prueba.
- Ningún agente se publica sin pasar sus evals.
- Cada cliente está aislado: su repo, su proyecto de Vercel, su proyecto de Supabase y sus claves.

## Si te trabás

Si en media hora no avanzás, escribí en el issue qué probaste y qué error te dio. Pedir ayuda temprano ahorra sesiones.
