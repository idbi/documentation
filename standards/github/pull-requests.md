# Solicitudes de cambio

El estilo de las solicitudes de cambio está considerado para que brinde más contexto y facilite la revisión de las mismas.

## Formato

### Título

Deber estar conformado por el prefijo seguido del código de la _card_ de Youtrack y luego el título de la solicitud de cambio. Tanto el prefijo como el código de la _card_ desde estar dentro de corchetes separados por un guión. El título debe ser corto, puede ser el mismo nombre de la _card_ de Youtrack, aunque deberá ser modificado o reemplazado si es muy largo.

#### Prefijos

- `HOTFIX`: Para correcciones urgentes de bugs (producción)
- `FIX`: Para correcciones urgentes de bugs (_dev_)
- `QW`: Para desarrollo de quick wins
- `HU`: Para historias de usuario
- `STAR`: Para mejoras que no son historias de usuario o quick wins
- `SYNC`: Para sincronizar ramas (producción o _dev_)

```
[PREFIJO - POS-#] Título
```

### Descripción

Debe contener información relevante sobre los cambios que se desean introducir.

#### Motivo

En esta sección debe ir una explicación breve de por qué se hicieron los cambios. También se debe adjuntar el enlace a la _card_ de Youtrack

#### Describe los cambios

En esta sección debe ir una explicación breve sobre qué cambios se hicieron.

#### Pruebas

En esta sección debe ir capturas, archivos, enlaces, etc.

```
## Motivo

...

> [POS-#](https://youtrack.idbi.pe/issue/POS-#) Título de card de Youtrack

## Describe los cambios

...

## Pruebas

...
```
