# **Ejercicio**: Crea ramas, modifica archivos y resuelve un conflicto
Ejercicio práctico para aplicar los conceptos aprendidos.

| Autor            | Fecha        | Día |
|------------------|--------------|----------|
| **Carlos Vásquez** |04 Noviembre 2025 | 4 |

## Crear y trabajar con ramas:

```sh
# Crear rama para feature
git checkout -b feature-analisis-ventas

# Modificar archivo
echo "# Análisis de ventas mejorado" >> README.md
git add README.md
git commit -m "feat: Agregar sección de análisis de ventas"

# Cambiar a rama main y crear conflicto
git checkout main
echo "# Análisis de datos principal" >> README.md
git add README.md
git commit -m "feat: Agregar análisis de datos principal"

```

## Crear conflicto y resolverlo:

```sh
# Intentar merge (creará conflicto)
git merge feature-analisis-ventas

# Ver archivos conflictivos
git status

# Editar archivo para resolver conflicto
# (eliminar marcadores de conflicto y elegir versión correcta)

# Completar merge
git add README.md
git commit -m "Merge: Resolver conflicto entre análisis de ventas y datos"

```

## Crear Pull Request:

- Push ambas ramas a GitHub
- Crear PR desde feature-analisis-ventas hacia main
- Agregar descripción y solicitar revisión
- Verificación: Confirma que el merge se completó exitosamente y que el historial refleja la resolución del conflicto.

### Requerimientos:
- Git configurado y conectado con GitHub (de días anteriores)
- Repositorio local con commits previos
-Editor de texto para resolver conflictos

