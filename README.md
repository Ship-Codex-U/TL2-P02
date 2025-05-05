# Practica 02

Realizar un analizador sintáctico que reconozca sentencias de asignación u operaciones simples,  y valide su estructura con una gramática como la siguiente (ejemplo):
<program>  -> <assignment> | <assignment> <program>
<assignment> -> <identifier> = <expression> ;
<identifier>   -> [a-zA-Z][a-zA-Z0-9_]*
<expression> -> <term> | <term> + <expression> | <term>
<expression>
<term>       -> <factor> | <factor> * <term> | <factor> / <term>
<factor>     -> <identifier> | <number> | ( <expression> )
<number>     -> [0-9]+


Pueden usar arboles sintácticos, tablas de derivación y/o autómatas. Se pueden apoyar con herramientas y librerias como yacc, o bison


## Descarga he instalación/configuración del proyecto

Clonar  repositorio

```bash
git clone
```

## Settear ambiente local
(Version de python: 3.12.1)

1. Crear un entorno virtual con **venv** dentro de la nueva carpeta que se creo al clonar el proyecto.

```bash
python -m venv nombre-entorno-virtual
```

2. Activar el entorno virtual creado.
```bash
nombre-entorno-virtual\Scripts\activate
```

3. Instalar los paquetes necesarios que requiere el proyecto para funcionan que vienen indicados en el archivo **requirements.txt**.
```bash
pip install -r requirements.txt
```

Nota: la aplicación para realizar y editar la interfaz del proyecto (Qt Design - design.exe) lo podras encontrar dentro de tu entorno virtual en la siguiente ruta
```bash
entorno-virtual-creado/Lib/Pyside6/
```

## Antes de realizar tu primer push.......
Asegurate que en tu archivo **.gitignore** aparezca por lo menos el siguiente renglon:

nombre-entorno-virtual-creado/  <------------ para que al momento de subir tus cambios no subas paquetes y librerias innecesarios a la repo que hagan que pese de mas.