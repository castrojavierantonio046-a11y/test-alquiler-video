# test-alquiler-video
Este proyecto implementa una API REST para una tienda virtual de videos, construida con lenguaje de programación Python y el framework FastApi. El objtivo es gestionar un catalogo de discos (peliculas o videos digitales) junto co0n las opoeraciones de registros de usuarios, vents y alquileres 

## Estructura del proyecto
|--Main.py #Punto de entrada de la aplicacion de la API, FastApi
|
  entidades/    #Directorion de paquetes que contiene todas las clases
  |- __init__.py
  |- disco.py
  |- usuario.py
  |- venta.py
  |- alquiler.py
  |- catalogo.py
##Instalacion y ejecucion
  1. Clonar el repositorio
     git clone https://github.com/usuario/test-alquiler-video.git
  2. cd test-alquiler-video
  3.  Crear y activar entorno virtual (opcoional, recomendado)
  4.  python -m venv venv
  5.  source venv/bin/activate #Linux/Mac
  6.  venv\Scripts\activate #Windows
  7.  Instalar dependecias
     7.1 pip install fastapi uvicorn pydantic
  10. Ejecutare el servidor
      10.1 uvicorn man:app --reload
  11. Acceder a la API
      *Documentacion interactiva: http//127.0.0.1:8000/docs
      *Documentacion alternativa (ReDoc):http://127.0.0.1:8000/redoc

##Endpoints principales (version inicial)
Metodo Endpoint Descripcion
GET    /discos/ Lista los discos disponibles
POST   /discos/ Agregar un nuevo disco
PUT    /discos/{id} Actualizar información de un disco
DELETE /discos/{id} Eliminar un disco
POST   /usuarios/ Registrar de nuevo usuario
POST   /ventas/  Registrar ventas
POST   /alquileres/ Registrar un alquiler

## Tecnologías utilizadas 
*Python 3.12.8
*FastAPI                                    
*Uvicorn (Servidor ASGI)

## Proyecto desarrollado como casa de estudio
* Nombre: **Javier Castro O.** <castrojavierantonio046@gmail.com>
* Github: castrojavierantonio046-a11y
