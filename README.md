cd ~/"herramientas computacionales"/JuegoVibora/pacman-game
cat > README.md << 'EOF'
Herramientas Computacionales - Pacman Game

 Descripcion

Este repositorio contiene una version extendida del juego "Pacman" de
la libreria freegames (Grant Jenks), un juego clasico de arcade hecho
con la libreria turtle de Python.

El jugador controla a Pacman con las flechas del teclado, moviendose
por un laberinto para comer toda la comida blanca mientras evita a los
4 fantasmas rojos que se mueven por el tablero.

Cambios realizados

- Commit 1: Estado inicial del proyecto, tal como se descarga de
  freegames (Grant Jenks), sin modificaciones.
- Commit 2: Se hizo que los fantasmas sean mas listos: en vez de
  elegir una direccion al azar al chocar con una pared, el 70% de las
  veces eligen la direccion valida que mas los acerca a Pacman. El 30%
  restante sigue siendo al azar, para que el juego no sea imposible.
- Pull Request: se cambio el tablero
  del laberinto y se aumento la velocidad de los fantasmas.

Como ejecutarlo

1. Crear un ambiente virtual: `python3 -m venv venv`
2. Activarlo: `source venv/bin/activate`
3. Instalar freegames: `pip install freegames`
4. Correr el juego: `python3 pacman.py`

 Controles

- Flechas del teclado: mueven a Pacman (Arriba, Abajo, Izquierda, Derecha)
- El puntaje se muestra en la esquina superior derecha
- El juego termina si un fantasma toca a Pacman
EOF
git add README.md
git commit -m "Add README with project description"
git push origin main
