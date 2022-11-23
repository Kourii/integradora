# Evaluación

El examen deber ́a realizarse en los plazos estipulados en la plataforma.
Se realizara en grupos de 2 personas, no mas.

## Consignas

Se desea realizar un control de tiempo de cocci ́on para un horno panadero, que permita
el encendido del quemador, ventilador de recirculacion y la inyeccion de vapor al horno.
Para esto se dispone de:

* 1 display que indicaran el tiempo de cocci ́on en minutos ( 0 a F, hexadecimal)
* 4 leds indicando la salida activa (quemador, ventilador, v ́alvula de vapor y un buzzer)
* 2 pulsadores que permiten ajustar el tiempo deseado
* 1 pulsador que comienza el tiempo, y permite pausar.
* 1 pulsador que permite cancelar el tiempo.

> Nota: Se busca minimizar las lineas que van del micro controlador al panel de display, para
ello utilice un registro de desplazamiento para el manejo de las salidas o las entradas, a
elecci ́on suya.

### El funcionamiento debe ser el siguiente:

1. Debe poder ajustarse el tiempo solo cuando este no esta corriendo o en pausa, es decir
cuando el horno esta en espera.
2. Un pulsador permitir ́a comenzar la cuenta regresiva o bien pausara/reanudara si ya hab ́ıa
comenzado.
3. Un pulsador permite cancelar en cualquier momento la cuenta regresiva y regresar a el
estado de espera.
4. Mientras el horno esta en espera, las salidas deben estar apagadas. Al comenzar la cuenta
regresiva se enciende el quemador y el ventilador.
5. Cuando se alcanzan las 3/4 partes del tiempo (puede ser aproximado), se debe activar la
v ́alvula de vapor.
6. Mientras el tiempo este pausado, se debe apagar el ventilador.
