# Documentación de variables de entorno

## Estilo de escritura

Usar `UPPER_SNAKE_CASE` para el nombre de las variables.

```text
DB_CONNECTION
```

## Agrupación de variables

Agrupar las variables por **funcionalidad**.

```text
DB_DATABASE=id_pos
DB_USERNAME=root
DB_PASSWORD=root

AUDIT_CONNECTION=mongodb
```

## Uso de variables de entorno

Usar el helper `config()` en lugar del helper `env()` para llamar a las variables de entorno.

Es necesario definir en que archivo de configuración localizarás las variables de entorno a usar. Estas se encuentran en la carpeta `config`.

```php
<?php
// config/app.php

return [

    'name' => env('APP_NAME', 'Laravel'),
    ...
];
```

## Valor de las variables

### Uso de comillas

Usar **comillas dobles** para los valores de las variables de entorno siempre que se haga referencia a otra variable o existan espacios en blanco.

```text
VARIABLE_WITH_BLANK_SPACES="IDBI growth up"
REFERENCE_TO="$VARIABLE_WITH_BLANK_SPACES all years"
```

### Referencias a otras variables

Es posible hacer referencias a otras variables.

### Tokens y Keys

**No usar** valores de **tokens** o **keys** sin el previo aviso y/o confirmación.

## Adición de nuevas variables

Cuando se agregue una nueva variable de entorno, ésta deberá ser puesta al final del archivo `.env.local.example` y `.env.production.example`.
