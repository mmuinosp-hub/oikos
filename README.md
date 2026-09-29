# OIKOS

Versión de desarrollo del simulador.

## Arranque local

```bash
npm install
npm start
```

Abrir `http://localhost:3000/`.

## Historial

Las sesiones terminadas se guardan dentro de `estado_actual.json` en `historialSesiones`. Además se conserva una copia de seguridad en `historiales/`.

Una sesión pasa al historial cuando el administrador cierra la producción y comienza una nueva sesión.

Las consolas solicitan explícitamente el historial al servidor mediante `solicitarHistorial`, por lo que no dependen de una actualización previa del navegador.

## Calculadora

La calculadora del jugador muestra producción y desperdicio de trigo y hierro. Para los procesos 1 y 2, el desperdicio corresponde al insumo que queda fuera de la proporción necesaria del proceso. El proceso 3 no tiene desperdicio.
