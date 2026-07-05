# Laboratorio 3: Copiloto de Código Eficiente

**Módulo:** 4 — Herramientas y Aplicaciones Prácticas
**Duración estimada:** 20 min
**Tipo:** Ejercicio práctico individual (nivel técnico)
**Herramientas:** Visual Studio Code + GitHub Copilot

---

## Objetivos

Al completar este laboratorio, podrás:

- Usar el comando `@workspace /explain` para que la IA analice la lógica de un archivo
- Solicitar de forma iterativa la generación de unit tests automáticos para una función
- Documentar código usando estándares limpios a través de atajos del IDE

---

## ¿Qué vas a necesitar?

- Visual Studio Code instalado (code.visualstudio.com)
- Extensión **GitHub Copilot** y **GitHub Copilot Chat** instaladas y activas
- Una cuenta de GitHub con Copilot habilitado
- Python 3 instalado (para ejecutar los tests)
- Una carpeta vacía creada en tu equipo para este laboratorio

---

## ¿Por qué es importante este laboratorio?

Copilot no es solo autocompletado. Con los comandos de chat adecuados y los atajos del IDE, puede analizar tu código, explicar su lógica, generar tests y documentarlo sin que tengas que escribir todo desde cero. Esto transforma el flujo de desarrollo: menos tiempo en tareas mecánicas y más en decisiones de diseño.

> Copilot es un becario brillante: su output hay que revisarlo, pero acelera drásticamente tareas repetitivas.

---

## Actividad 1: Prepara el código de prueba (3 min)

### Paso 1: Crea y abre la carpeta del proyecto

1. Crea una carpeta nueva en tu equipo, por ejemplo: `lab3-copiloto`
2. Abre VS Code y haz clic en **File > Open Folder...** (o **Archivo > Abrir carpeta...**)
3. Selecciona la carpeta que acabas de crear

> `@workspace` solo funciona si tienes una carpeta abierta en VS Code, no un archivo suelto. Al abrir la carpeta, VS Code crea automáticamente un workspace.

### Paso 2: Crea el archivo con el código

Copia y pega esta función en un nuevo archivo `calculos.py` dentro de la carpeta:

```python
def calc(a, b, c, d):
    r = 0
    if c == '+':
        r = a + b
    elif c == '-':
        r = a - b
    elif c == '*':
        r = a * b
    elif c == '/':
        if b != 0:
            r = a / b
        else:
            r = 'error'
    if d == 1:
        r = r * 1.21
    elif d == 2:
        r = r * 1.04
    return r
```

> Esta función tiene malas prácticas: nombres poco descriptivos, sin comentarios, lógica mezclada y propósito poco claro. Trabajarás con ella durante todo el laboratorio.

**Marca cuando lo hayas hecho:**
- [ ] Creé el archivo `calculos.py` con el código
- [ ] Lo abrí en VS Code

---

## Actividad 2: Analiza el código con @workspace /explain (4 min)

### Paso 1: Abre Copilot Chat

Haz clic en el icono de Copilot Chat en la barra lateral de VS Code (el icono del chat con estrellas).

También puedes usar el atajo de teclado: `Ctrl+Shift+I` (Windows/Linux) o `Cmd+Shift+I` (Mac).

### Paso 2: Usa @workspace /explain

Escribe **exactamente** este comando en el chat de Copilot y pulsa Enter:

> `@workspace /explain ¿Qué hace la función calc? Describe su lógica, parámetros y posibles problemas de diseño.`

El comando `@workspace` le dice a Copilot que analice todo tu proyecto. El comando `/explain` le pide que explique el código paso a paso.

**Pega aquí la explicación que te dio Copilot:**
> _________________________________________________________________
> _________________________________________________________________
> _________________________________________________________________

### Paso 3: Pregunta de seguimiento

Ahora haz una segunda pregunta para profundizar. Escribe en el mismo chat:

> `¿Qué nombres de variables y función sugerirías para que el código sea más legible y siga las convenciones de Python (PEP 8)?`

**Pega aquí las sugerencias de Copilot:**
> _________________________________________________________________
> _________________________________________________________________

**Responde:**
1. ¿Copilot entendió correctamente la lógica de la función? ______
2. ¿Las sugerencias de nombres siguen snake_case (PEP 8)? ______
3. Antes de este laboratorio, ¿habías usado `@workspace /explain`? ______

---

## Actividad 3: Refactoriza el código con IA (4 min)

### Paso 1: Pide la refactorización

Ahora vas a pedir a Copilot que reescriba la función correctamente. Escribe en el chat:

> `Refactoriza la función calc para que tenga nombres descriptivos en snake_case, use match-case (Python 3.10+), constantes para los tipos de IVA, type hints y maneje errores correctamente. Devuélveme el código completo refactorizado.`

**Pega aquí el código refactorizado que te devolvió:**
> _________________________________________________________________
> _________________________________________________________________
> _________________________________________________________________
> _________________________________________________________________

### Paso 2: Reemplaza el código

Selecciona TODO el contenido de `calculos.py` (`Ctrl+A` / `Cmd+A`) y pégalo encima con el código refactorizado que te dio Copilot.

**Marca cuando lo hayas hecho:**
- [ ] Copilot me devolvió el código refactorizado
- [ ] Reemplacé el contenido del archivo

---

## Actividad 4: Genera unit tests iterativamente (5 min)

### Paso 1: Crea el archivo de test vacío

Pulsa `Ctrl+N` (o `Cmd+N`) para crear un archivo nuevo. Guárdalo como `test_calculos.py` en la misma carpeta (`Ctrl+S` / `Cmd+S`).

### Paso 2: Primera iteración — tests básicos

Escribe en el chat de Copilot:

> `@workspace Genera unit tests con pytest para la función del archivo calculos.py. Empieza con los casos básicos: suma, resta, multiplicación y división exacta.`

Espera la respuesta. Copia el código y pégalo en `test_calculos.py`.

**Pega aquí los tests básicos que te generó:**
> _________________________________________________________________
> _________________________________________________________________

### Paso 3: Segunda iteración — añade casos borde

Ahora, sin borrar lo anterior, escribe en el chat:

> `Añade más tests para cubrir: división entre cero, IVA 21% e IVA 4%. Los tests adicionales deben usar las mismas convenciones que los anteriores.`

Copia SOLO los tests nuevos y pégalos al final de `test_calculos.py`.

**Pega aquí los tests adicionales:**
> _________________________________________________________________
> _________________________________________________________________

### Paso 4: Ejecuta los tests

Abre la terminal integrada de VS Code (`Ctrl+ñ` o `Cmd+ñ`) y ejecuta:

```bash
pip install pytest
pytest test_calculos.py -v
```

**Resultado de la ejecución (tests pasados/fallados):**
> _________________________________________________________________

**Responde:**
1. ¿Los tests cubren todos los casos que pediste? ______
2. ¿Hubo algún test que fallara? ¿Por qué? ______
3. ¿Notas la diferencia entre pedir todo de golpe vs. hacerlo iterativamente? ______

---

## Actividad 5: Documenta el código con atajos del IDE (4 min)

### Paso 1: Genera el docstring con el atajo inline

Selecciona toda la función con el ratón y en el chat escribe:

> `Añade un docstring Google-style a esta función explicando qué hace, cada parámetro (Args), el valor de retorno (Returns) y ejemplos de uso (Examples). Sigue PEP 257.`

**Pega aquí la función con el docstring generado:**
> _________________________________________________________________
> _________________________________________________________________
> _________________________________________________________________
> _________________________________________________________________

### Paso 2: Documenta los tests

Abre `test_calculos.py`. Selecciona todo el archivo y en el chat escribe:

> `Añade un docstring al módulo y comentarios descriptivos antes de cada función de test explicando qué caso prueban.`

**Pega aquí el resultado:**
> _________________________________________________________________
> _________________________________________________________________

**Marca cuando lo hayas hecho:**
- [ ] La función principal tiene docstring Google-style
- [ ] El archivo de tests tiene docstring de módulo y comentarios
- [ ] Ambos archivos están guardados

---

## Resumen del laboratorio

- [ ] Creé el archivo `calculos.py` con código sin optimizar
- [ ] Usé `@workspace /explain` para que Copilot analizara la lógica del archivo
- [ ] Refactoricé el código con IA
- [ ] Generé unit tests de forma iterativa (básicos + casos borde) con pytest
- [ ] Documenté el código con docstrings usando atajos del IDE

---

## Soluciones

### Actividad 2 — ¿Qué debería explicar Copilot? [↑ Volver](#actividad-2-analiza-el-código-con-workspace-explain-4-min)

Copilot debería identificar que la función:
- Recibe dos operandos (`a`, `b`), un operador (`c`) y un tipo de IVA (`d`)
- Realiza una operación aritmética básica (suma, resta, multiplicación, división)
- Aplica un IVA del 21% (si `d == 1`) o del 4% (si `d == 2`)
- No valida tipos de entrada, tiene nombres poco descriptivos, no usa type hints, y mezcla lógica aritmética con fiscal

### Actividad 3 — Ejemplo de refactorización [↑ Volver](#actividad-3-refactoriza-el-código-con-ia-4-min)

```python
IVA_21 = 1.21
IVA_04 = 1.04

def calcular_precio_final(precio1: float, precio2: float,
                          operador: str, tipo_iva: int) -> float | str:
    match operador:
        case '+': resultado = precio1 + precio2
        case '-': resultado = precio1 - precio2
        case '*': resultado = precio1 * precio2
        case '/':
            if precio2 == 0:
                return 'Error: división entre cero'
            resultado = precio1 / precio2
        case _: return 'Error: operador no válido'

    if tipo_iva == 1:
        resultado *= IVA_21
    elif tipo_iva == 2:
        resultado *= IVA_04

    return round(resultado, 2)
```

### Actividad 4 — Tests esperados [↑ Volver](#actividad-4-genera-unit-tests-iterativamente-5-min)

**Primera iteración (tests básicos):**
```python
def test_suma_sin_iva():
    assert calcular_precio_final(100, 50, '+', 0) == 150

def test_resta_sin_iva():
    assert calcular_precio_final(100, 30, '-', 0) == 70

def test_multiplicacion_sin_iva():
    assert calcular_precio_final(10, 5, '*', 0) == 50

def test_division_exacta():
    assert calcular_precio_final(100, 4, '/', 0) == 25
```

**Segunda iteración (casos borde):**
```python
def test_division_entre_cero():
    assert calcular_precio_final(10, 0, '/', 0) == 'Error: división entre cero'

def test_iva_21():
    assert calcular_precio_final(100, 0, '+', 1) == 121

def test_iva_04():
    assert calcular_precio_final(100, 0, '+', 2) == 104

def test_operador_invalido():
    assert calcular_precio_final(10, 5, '^', 0) == 'Error: operador no válido'
```

### Actividad 5 — Docstring esperado [↑ Volver](#actividad-5-documenta-el-código-con-atajos-del-ide-4-min)

```python
def calcular_precio_final(precio1: float, precio2: float,
                          operador: str, tipo_iva: int) -> float | str:
    """Calcula el resultado de una operación aritmética entre dos precios
    y opcionalmente aplica un porcentaje de IVA.

    Args:
        precio1: Primer operando (precio base).
        precio2: Segundo operando (precio adicional o divisor).
        operador: Operador aritmético ('+', '-', '*', '/').
        tipo_iva: Tipo de IVA (0=ninguno, 1=21%, 2=4%).

    Returns:
        Resultado del cálculo redondeado a 2 decimales,
        o un mensaje de error si la operación no es válida.

    Examples:
        >>> calcular_precio_final(100, 50, '+', 1)
        181.5
        >>> calcular_precio_final(10, 0, '/', 0)
        'Error: división entre cero'
    """
```

---

[Volver a laboratorios](index.md)
