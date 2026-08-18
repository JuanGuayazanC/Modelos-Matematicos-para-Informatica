# Modelos Matemáticos para Informática (MMIN)

Repositorio general del curso Modelos Matemáticos para Informática, que agrupa —mediante submódulos de git— los talleres y recursos del curso.

Cada submódulo es un repositorio independiente con su propio historial de commits y README. Para saber cómo aprovechar este repositorio, ver [Cómo usar este repositorio](#cómo-usar-este-repositorio).

## Estructura del proyecto

```
Modelos-Matematicos-para-Informatica/
├── Talleres/
│   ├── Suma-Recursiva-Haskell-MMIN/
│   └── Manipulacion-de-Digitos-en-Haskell-MMIN/
└── Recursos/
    ├── Sistema-Formal-a-b-M-MMIN/
    ├── Sistema-Formal-I-M-MMIN/
    ├── Sistema-Formal-IMIII-MMIN/
    └── Sistema-Formal-Sapos-y-Ranas-MMIN/
```

## Temas del curso

El curso recorre los fundamentos matemáticos discretos aplicados a la informática, con dos grandes bloques de contenido:

- **Sistemas formales**: sistemas de producción (Post), reglas de reescritura de cadenas, y su aplicación a problemas clásicos como el rompecabezas de sapos y ranas y variantes del sistema MIU.
- **Programación funcional (Haskell)**: recursión, guardas, y manipulación de dígitos de números mediante operaciones aritméticas (`div`/`mod`).

## Cosas a tener en cuenta

- Los 4 repositorios de `Recursos/` son trazas de derivación de sistemas formales generadas con la herramienta `SISFOR` (`sisfor.EXE`, DOS) — no son código Prolog ejecutable por sí solo, sino el formato de datos que usa esa herramienta.
- El código de los talleres provino de documentos Word (`.docx`) donde el código Haskell estaba pegado como texto; se extrajo tal cual a archivos `.hs`.

## Herramientas

- Haskell (GHC/runghc)
- SISFOR (simulador de sistemas formales/producción, DOS)

## Profesor

Wilmer Edicson Garzón Alfonso.

## Cómo usar este repositorio

Este repositorio no contiene código directamente: es una colección de repositorios independientes (talleres y recursos), organizados por carpetas. Cada carpeta es un submódulo de git que apunta al repositorio real de esa actividad.

- **Para consultar una actividad puntual**: entra directamente a su carpeta en GitHub (o navega el submódulo) y revisa su propio README.
- **Para tener todo el contenido en tu máquina**:

```bash
git clone --recurse-submodules https://github.com/JuanGuayazanC/Modelos-Matematicos-para-Informatica.git
```

Si ya clonaste el repositorio sin submódulos:

```bash
git submodule update --init --recursive
```
