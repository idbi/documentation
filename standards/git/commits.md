# Commits

El estilo de los commits sigue los commits convencionales en repositorios open source.

## Formato de los commits

Los commits están compuestos por un **prefijo** seguido de dos puntos (`:`), entre corchetes el **identificador de la card** asociada al commit (opcionalmente un número **para indicar el orden**) y finalmente un mensaje.
Opcionalmente puede agregarse una **descripción** en la segunda línea y un `close #?` para cerrar una `issue` en la tercera línea.

```
<prefijo>: [POS-#] <mensaje>
<descripción?>
```

**Nota:** En el `POS-#`, el `#` indica el número de la _card_ asociada.

Aquí algunos ejemplos:

> feat: [POS-10040] handle toppings, discounts and combo extra prices

> feat: [POS-10034] create getExtraComboPrice function
> Some description

Si existen más commits asociadas a una card, se pueden ordenar agregando números al final del identificador de la card.
El primer commit asociado **no posee un número**, pero se entenderá que es el primero:

> feat: [POS-10034] create getExtraComboPrice function
> feat: [POS-10034-2] update getExtraComboPrice function

## Lista de prefijos disponibles

- `build`: Cambio que afectan al build del sistema o dependencias externas (ejemplos: gulp, broccoli, npm).
- `ci`: Cambios para archivos de configuración de CI y scripts (ejemplos: Travis, Circle, BrowserStack, SauceLabs).
- `chore`: Cambios que no cambian el código fuente o tests. Por ejemplo cambios al proceso de build, herramientas auxiliares, actualizaciones o nuevas dependencias.
- `docs`: Solo cambios en la documentación (por ejemplo, en el README, en storybooks).
- `feat`: Una nueva funcionalidad.
- `fix`: Una corrección de un bug.
- `perf`: Un cambio en el código que mejora la performance
- `refactor`: Un cambio en el código que no corrige un bug ni añade un funcionalidad
- `revert`: Al revertir un cambio :+1:.
- `style`: cambios que no afectan el significado del código (espacios en blanco, formateo, sin `;` al final de una línea, etc).
- `test`: Para agregar nuevos tests o corregirlos.
