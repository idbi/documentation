# Commits

El estilo de los commits sigue los commits convencionales en repositorios open source.

## Formato de los commits

### Asunto

El asunto de los commits están compuestos por un **prefijo** seguido de dos puntos (`:`), entre corchetes el **identificador de la card** asociada al commit (opcionalmente un número **para indicar el orden**) y finalmente un **mensaje**.

El **mensaje** del asunto explica el **como** de lo que se ha realizado.

Debe considerarse:

- Limitar la línea de asunto a **50 caracteres** (sin considerar el prefijo ni el identificador de la card).
- Poner en mayúscula la primera letra del **mensaje** del asunto.
- Usar el [estado de ánimo imperativo](https://midu.dev/buenas-practicas-escribir-commits-git/) en el **mensaje** del asunto (escribir los verbos en tiempo _presente_.)

### Descripción

Opcionalmente puede agregarse una **descripción** en la segunda línea y un `close #?` para cerrar una `issue` en la tercera línea.

La **descripción** explica el **qué** y el **por qué** de lo que se ha realizado.

Debe considerarse:

- Separar el asunto de la descripción con una línea en blanco.
- Limitar la línea de la descripción a **72 caracteres**.

### Resumen

```
<prefijo>: [POS-#] <mensaje>

<descripción?>
```

**Nota:** En el `POS-#`, el `#` indica el número de la _card_ asociada.

### Ejemplos

Aquí algunos ejemplos:

> feat: [POS-10040] handle toppings, discounts and combo extra prices

> feat: [POS-10034] create getExtraComboPrice function
>
> I have to create extra function to get the extra combo price because the
> service does not provide a method to do this and it can be reusable in
> other places like events or jobs

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
