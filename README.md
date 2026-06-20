# Tanque de Equilibrio

**Tanque de Equilibrio** es un minijuego educativo de física desarrollado como parte del proyecto **EulerGames**. El juego simula un tanque cilíndrico que se llena mediante un caudal de entrada controlado por el usuario, mientras pierde agua por un orificio lateral ubicado en la parte baja del tanque.

El objetivo del jugador es calcular qué porcentaje del caudal máximo debe abrir para que el nivel del agua se estabilice en una altura solicitada.

---

## Objetivo educativo

El juego está diseñado para que el estudiante analice un sistema de flujo en equilibrio dinámico. No se trata simplemente de llenar el tanque hasta cierta altura, sino de encontrar el caudal de entrada que permite que el nivel del agua se mantenga estable cuando el caudal de salida iguala al caudal de entrada.

El estudiante debe interpretar datos físicos, realizar cálculos en su libreta y probar su respuesta dentro de la simulación.

---

## Conceptos físicos involucrados

El juego trabaja principalmente con:

* continuidad de caudal;
* presión hidrostática;
* salida de agua por un orificio lateral;
* velocidad de salida tipo Torricelli;
* coeficiente de descarga;
* equilibrio dinámico entre entrada y salida;
* evolución temporal del nivel de agua en un tanque.

La simulación considera que el caudal de salida aumenta conforme sube el nivel del agua, ya que la presión sobre el orificio lateral se incrementa.

---

## Mecánica del juego

Cada ronda genera aleatoriamente un tanque cilíndrico con dimensiones distintas, un orificio lateral de tamaño variable y una altura objetivo.

El usuario puede ajustar únicamente el porcentaje del caudal máximo mediante una perilla o controles de teclado. Una vez que presiona **Abrir caudal**, el valor elegido queda bloqueado y comienza la simulación.

El tanque inicia vacío. El agua entra por la parte superior y sale por el orificio lateral cuando el nivel supera la altura del orificio. El chorro de salida se representa de forma horizontal y su trayectoria cambia según la presión del agua en el tanque.

El jugador gana si el nivel del agua se estabiliza dentro de la tolerancia permitida alrededor de la altura objetivo.

---

## Datos visibles para el jugador

Antes de iniciar cada intento, el juego muestra:

* altura del tanque;
* diámetro del tanque;
* altura del centro del orificio;
* diámetro del orificio;
* coeficiente de descarga;
* caudal máximo disponible;
* altura objetivo;
* tolerancia permitida.

No se muestran fórmulas ni soluciones antes del intento.

---

## Retroalimentación

Después de la simulación, el juego muestra una retroalimentación física con:

* altura objetivo;
* altura de equilibrio alcanzada;
* error respecto al objetivo;
* caudal elegido;
* caudal de salida final;
* resultado de la ronda.

Además, el juego incluye un foco industrial de resultado:

* verde si el jugador acierta;
* rojo si falla.

También se aplica un brillo visual general a la interfaz para reforzar el resultado.

---

## Controles

### Perilla

El porcentaje del caudal puede ajustarse girando la perilla con el mouse.

### Teclado

* `←` disminuye el caudal en 1%.
* `→` aumenta el caudal en 1%.
* `↓` disminuye el caudal en 0.1%.
* `↑` aumenta el caudal en 0.1%.
* `Enter` o `Espacio` abre el caudal o continúa a la siguiente ronda.

### Botones

También se incluyen botones para ajuste grueso y fino, además del botón **Abrir caudal**.

---

## Características principales

* Juego ejecutable directamente en navegador.
* Desarrollado en un solo archivo `index.html`.
* Sin librerías externas.
* Simulación en tiempo físico real.
* Rondas aleatorias y físicamente resolubles.
* Tanque cilíndrico con dimensiones variables.
* Orificio lateral bajo con diámetro aleatorio.
* Caudal máximo calculado para garantizar solución.
* Chorro lateral parabólico dependiente del nivel del agua.
* Entrada de agua conectada visualmente con el agua almacenada.
* Interfaz con estética industrial.
* Retroalimentación posterior al intento.
* Foco industrial de acierto o fallo.
* Sonido opcional.

---

## Modelo físico simplificado

La altura del agua evoluciona según la diferencia entre el caudal de entrada y el caudal de salida.

El caudal de entrada depende del porcentaje elegido por el jugador respecto al caudal máximo disponible.

El caudal de salida depende del área del orificio, del coeficiente de descarga y de la altura de agua sobre el orificio.

Cuando el caudal de entrada y el caudal de salida se igualan, el nivel del agua se estabiliza.

---

## Filosofía EulerGames

Este juego forma parte de **EulerGames**, una colección de minijuegos educativos de física y matemáticas.

La filosofía del proyecto es que los juegos no sean simulaciones pasivas ni ejercicios resueltos automáticamente. El estudiante debe:

1. leer los datos físicos;
2. calcular en su libreta;
3. tomar una decisión;
4. probar su respuesta;
5. recibir retroalimentación física después del intento.

El juego busca funcionar como un reto interactivo, no como una calculadora disfrazada.

---

## Cómo usar

Solo es necesario abrir el archivo:

```text
index.html
```

en cualquier navegador moderno.

No requiere instalación, servidor local ni dependencias externas.

---

## Tecnologías utilizadas

* HTML
* CSS
* JavaScript
* Canvas API

---

## Estado del proyecto

Versión inicial funcional del minijuego **Tanque de Equilibrio**.

El juego ya incluye la mecánica principal, simulación física, controles, retroalimentación visual y generación aleatoria de rondas.
