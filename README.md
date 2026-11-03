# Asteroids

Clon del clásico arcade **Asteroids** implementado en canvas HTML5 puro, sin dependencias ni bundler.

## Descripción

Nave espacial en un campo de asteroides con envolvimiento de bordes (el espacio es toroidal). Destruye asteroides para sumar puntos: los grandes se parten en medianos, los medianos en pequeños. Al destruirlos puede aparecer un power-up de **Velocidad**. Cada nivel incluye además una **estrella fugaz**, un asteroide especial que cruza el campo a gran velocidad y desaparece al agotar su tiempo.

## Tecnologías

- **HTML5 Canvas** — renderizado 2D
- **JavaScript (ES6+)** — lógica del juego en un solo archivo `game.js`
- Sin frameworks, sin bundler, sin dependencias

## Cómo correr

Abre `index.html` directamente en el navegador (doble clic), o usa un servidor local:

```bash
npx serve .
```

Luego visita `http://localhost:3000`.

## Controles

| Tecla     | Acción     |
| --------- | ---------- |
| `←` `→`   | Rotar nave |
| `↑`       | Propulsar  |
| `Espacio` | Disparar   |

## Puntuación

| Asteroide      | Puntos |
| -------------- | ------ |
| Grande         | 20     |
| Mediano        | 50     |
| Pequeño        | 100    |
| Estrella fugaz | 150    |

## Power-ups

| Power-up  | Efecto                                          | Duración |
| --------- | ----------------------------------------------- | -------- |
| Velocidad | Duplica la velocidad de desplazamiento de la nave | 5 s      |

- Al destruir un asteroide hay un 15 % de probabilidad de que aparezca un rayo amarillo.
- Si no se recoge, desaparece a los 10 segundos.
- Recoger otro mientras el efecto está activo reinicia el contador a 5 segundos.
- El efecto se pierde al recibir un impacto y se muestra el tiempo restante en el HUD.

## Características

- 3 vidas con invencibilidad temporal al reaparecer (parpadeo)
- Asteroides se parten en fragmentos más pequeños al ser destruidos
- Partículas de explosión al destruir asteroides
- Power-up de Velocidad con indicador de tiempo restante en el HUD
- Estrella fugaz por nivel, con estela luminosa, 150 puntos y 8 segundos de vida
