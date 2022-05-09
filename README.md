# SemanaTec
# 1. HEADER
## - Gerardo Mora Beltrán - A00827128 - ITC - Semestre 6
### - Los Mochis, Sinaloa

**2. Bold**

*3. Italica*
> blockquote

Lista ordenada de mis platillos favoritos
1. Enchiladas suizas
2. Hamburguesas
3. Kimchi bokkeumbap
4. Fetuccine alfredo
5. Tacos de trompo
6. Sushi
7. Flan
8. Pizza

Lista desordenada de sus momentos del Día de la Madre
- Carta
- Dibujo de ambos
- Librito con razones del porqué la amo tanto
- Corazoncitos

```python
"""Paint, for drawing shapes.

Exercises

1. Add a color.
2. Complete circle.
3. Complete rectangle.
4. Complete triangle.
5. Add width parameter.
"""

from turtle import *

from freegames import vector


def line(start, end):
    """Draw line from start to end."""
    up()
    goto(start.x, start.y)
    down()
    goto(end.x, end.y)


def square(start, end):
    """Draw square from start to end."""
    up()
    goto(start.x, start.y)
    down()
    begin_fill()

    for count in range(4):
        forward(end.x - start.x)
        left(90)

    end_fill()


def circle(start, end):
    """Draw circle from start to end."""
    pass  # TODO


def rectangle(start, end):
    """Draw rectangle from start to end."""
    pass  # TODO


def triangle(start, end):
    """Draw triangle from start to end."""
    pass  # TODO


def tap(x, y):
    """Store starting point or draw shape."""
    start = state['start']

    if start is None:
        state['start'] = vector(x, y)
    else:
        shape = state['shape']
        end = vector(x, y)
        shape(start, end)
        state['start'] = None


def store(key, value):
    """Store value in state at key."""
    state[key] = value


state = {'start': None, 'shape': line}
setup(420, 420, 370, 0)
onscreenclick(tap)
listen()
onkey(undo, 'u')
onkey(lambda: color('black'), 'K')
onkey(lambda: color('white'), 'W')
onkey(lambda: color('green'), 'G')
onkey(lambda: color('blue'), 'B')
onkey(lambda: color('red'), 'R')
onkey(lambda: store('shape', line), 'l')
onkey(lambda: store('shape', square), 's')
onkey(lambda: store('shape', circle), 'c')
onkey(lambda: store('shape', rectangle), 'r')
onkey(lambda: store('shape', triangle), 't')
done()
```

---
# Link
[Titulo](https://www.github.com)

# Imagen
![Imagen](https://i.pinimg.com/474x/74/61/7a/74617a0b84fc2cac8ede0f948791c628.jpg)

# Tabla
| Syntax | Description |
| ---------- | ------------ |
| Header | Title |
| Paragraph | Text |

# Actividades
- [X] Rutina circulo
- [ ] Triangulo pendiente
- [ ] Rectangulooo

H^2^

Practicar github
