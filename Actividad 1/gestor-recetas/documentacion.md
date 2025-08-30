1. Información general
Este proyecto es un ejercicio académico para aprender trabajo colaborativo con Git y GitHub, simulando el desarrollo de un Gestor de Recetas Digitales.
El trabajo se realizó usando Visual Studio Code, Git y GitHub siguiendo buenas prácticas de control de versiones.

2. Ramas creadas y responsables
main → Rama principal.
feature/recetas-colombianas → Responsable: Estudiante 1.
feature/recetas-mexicanas → Responsable: Estudiante 2.
feature/recetas-italianas → Responsable: Estudiante 3.
fix/colombianas-version1 → Rama para modificar colombianas (primera versión).
fix/colombianas-version2 → Rama para generar conflicto intencional.

3. Comandos utilizados
Inicialización del repositorio
git init
git add .
git commit -m "Estructura base del proyecto gestor de recetas"
git branch -M main
git remote add origin https://github.com/Johan16lindis/gestor-recetas.git
git push -u origin main

Creación de ramas
git checkout -b feature/recetas-colombianas
git checkout -b feature/recetas-mexicanas
git checkout -b feature/recetas-italianas

Commits de ejemplo
git add recetas/colombianas.md
git commit -m "Agregada receta: Bandeja paisa"
git commit -m "Agregada receta: Ajiaco"
git commit -m "Agregada receta: Sancocho"

Subida de ramas
git push origin feature/recetas-colombianas
git push origin feature/recetas-mexicanas
git push origin feature/recetas-italianas

Conflicto intencional
git checkout -b fix/colombianas-version1
# editar y commitear cambios
git checkout -b fix/colombianas-version2
# editar misma línea y commitear cambios

Tags
git tag v1.0.0
git push origin v1.0.0

4. Pull Requests y Merges
Cada rama de recetas (colombianas, mexicanas, italianas) se integró a main mediante Pull Requests en GitHub.
Se incluyeron al menos 3 commits por rama.
Cada PR fue aprobado y luego mergeado.

5. Conflicto generado y resuelto
Se creó un conflicto intencional en el archivo recetas/colombianas.md modificando la misma línea en dos ramas distintas (fix/colombianas-version1 y fix/colombianas-version2).
GitHub mostró el conflicto al intentar hacer el segundo Pull Request.
El archivo original se veía así:

Resolución final (combinando ambas versiones):

- Bandeja paisa con frijoles antioqueños, típica de Medellín
- Ajiaco
- Sancocho

6. Tag de versión final
Al finalizar el trabajo se creó el tag v1.0.0, marcando la primera versión estable del proyecto.

7. Conclusiones
Se comprendió el flujo de trabajo con Git y GitHub.
Se practicó la creación y uso de ramas por funcionalidad.
Se aprendió a realizar Pull Requests y revisiones.
Se resolvió un conflicto de manera manual en GitHub.
Se marcó una versión final del proyecto con un tag.

