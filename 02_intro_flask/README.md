### Introducción al lenguaje Python
Universidad ICESI  
Curso: Sistemas Operativos  
Docente: Daniel Barragán C.  
Tema: Introducción a servicios web con Python  
Correo: daniel.barragan at correo.icesi.edu.co

### Objetivos
* Crear servicios web por medio de Python
* Realizar pruebas sobre servicios web

### Introducción
Flask es un micro web framework escrito en Python y basado en la especificación WSGI de Werkzeug y el motor de templates Jinja2. Tiene licencia BSD.

### Instalación

Para la ejecución de los ejemplos se emplearán entornos virtuales.

```
# cd /tmp
# wget https://bootstrap.pypa.io/get-pip.py
# python get-pip.py
# pip install virtualenv
```

### Desarrollo

#### Crear un ambiente virtual

Cree un ambiente virtual

```
# su python_user
$ cd ~/
$ mkdir envs
$ cd envs
$ virtualenv flask_env
```

#### Activar un ambiente virtual

Active el ambiente virtual creado

```
$ cd ~/envs
$ . flask_env/bin/activate
```

#### Instalación de Flask

Con el ambiente activo, instale la libreria Flask

```
$ pip install Flask
```

#### Ejemplo básico

Cree un directorio para alojar los ejemplos

```
$ cd ~/
$ mkdir -p flask_examples/01_ejemplo_basico
$ cd flask_examples/01_ejemplo_basico
```

Cree un archivo de nombre hello.py

``` python
from flask import Flask
app = Flask(__name__)

@app.route("/greeting")
def hello():
    return "Hello World!"

if __name__ == "__main__":
    app.run(0.0.0.0)
```

```
$ python hello.py
```

#### Contrato REST

#### Implementación del contrato

#### Pruebas del servicio web

#### Desactivar un ambiente virtual

```
$ deactivate
```

### Actividades

