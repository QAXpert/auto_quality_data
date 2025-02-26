### Generación de Reporte Mensual para Envío de Notificaciones - Banco QAX

Este repositorio se centra en la automatización del proceso de generación de un reporte mensual para el envío de notificaciones de balances a los clientes del Banco QAX. La historia de usuario asociada a este proyecto es la siguiente:

**Historia de Usuario: Envío de Notificaciones Mensuales de Balances para Clientes del Banco QAX**

Como administrador del portal, quiero generar un reporte con los datos específicos de los clientes del Banco QAX para realizar los envíos mensuales de notificaciones de sus balances.

**Criterios de Aceptación:**
- El reporte debe incluir la columna "age" que solo permita valores numéricos y esté restringida al rango de 18 a 100 años.
- La columna "month" (Mes) debe contener exactamente 3 caracteres, representando el mes de la notificación.
- La columna "housing" solo puede tener dos respuestas posibles: "yes" o "no", indicando si el cliente tiene vivienda propia o no.


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
great_expectations --version
```

### Creacion del proyecto

```
great_expectations init
```

### Creación de Data Source

```
great_expectations datasource new
```

```
great_expectations datasource list
```


### Creación de Suite

```
great_expectations suite new --no-jupyter

```

```
great_expectations suite list

```

### Creación de Checkpoint

```
great_expectations checkpoint new run_testing_bank_qax
```

```
great_expectations checkpoint list
```

### Ejecución

```
great_expectations checkpoint run run_testing_bank_qax

```

El archivo de reporte que almacenado: 
great_expectations/uncommitted/data_docs/local_site/index.html

### Documentación de las validaciones

[Documentacion](https://greatexpectations.io/expectations/?viewType=Summary)

