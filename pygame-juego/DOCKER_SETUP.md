# 🎮 Juego con Pygame

## 📋 Descripción
Juego simple creado con Pygame que muestra cómo ejecutar aplicaciones gráficas en Docker.

## Observaciones
Cambiar la sección ENV DISPLAY=:0 en dockerfile con el display que se quiera utilizar

## 🚀 Cómo usar
# Construir la imagen
docker build -t pygame-juego .

# Ejecutar el contenedor
docker run -it --rm \
  -e DISPLAY=$DISPLAY \
  -v /tmp/.X11-unix:/tmp/.X11-unix \
  pygame-juego