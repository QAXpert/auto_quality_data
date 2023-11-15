### Generación de Reporte Mensual para Envío de Notificaciones - Banco QAX

Este repositorio se centra en la automatización del proceso de generación de un reporte mensual para el envío de notificaciones de balances a los clientes del Banco QAX. La historia de usuario asociada a este proyecto es la siguiente:

**Historia de Usuario: Envío de Notificaciones Mensuales de Balances para Clientes del Banco QAX**

Como administrador del portal, quiero generar un reporte con los datos específicos de los clientes del Banco QAX para realizar los envíos mensuales de notificaciones de sus balances.

**Criterios de Aceptación:**
- El reporte debe incluir la columna "Age" que solo permita valores numéricos y esté restringida al rango de 18 a 100 años.
- La columna "Mouth" (Mes) debe contener exactamente 3 caracteres, representando el mes de la notificación.
- La columna "Housing" solo puede tener dos respuestas posibles: "Yes" o "No", indicando si el cliente tiene vivienda propia o no.


### Formato del CSV para Generación del Reporte

| age | job          | marital | education | default | balance | housing | loan | contact  | day | month | duration | campaign | pdays | previous | poutcome | y   |
|-----|--------------|---------|-----------|---------|---------|---------|------|----------|-----|-------|----------|----------|-------|----------|----------|-----|
| 30  | unemployed   | married | primary   | no      | 1787    | no      | no   | cellular | 19  | oct   | 79       | 1        | -1    | 0        | unknown  | no  |


###  Pre-requisitos
- Python instalado (versión 3.11)
- PIP (Python Package Installer) instalado (23.0.1)

###  Configuración de Great Expectations

Este repositorio se centra en la automatización de pruebas de calidad de datos utilizando Great Expectations. Sigue los pasos a continuación para configurar y ejecutar el proyecto.

#### Instalación
```
pip3 install great_expectations
greate_expectations --version
```

### Creacion del proyecto

```
great_expectations init
```

### Creación de Data Source

```
great_expectations datasource new
```


### Creación de Suite

```
great_expectations suite new

```

### Edición de la suite 

```
great_expectations suite edit btest

```

### Creación de Checkpoint

```
great_expectations checkpoint new

```


### Ejecución

```
great_expectations run

```
