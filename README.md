# Calculadora del año óptimo de venta

Calculadora interactiva de inversión inmobiliaria (propiedad de renta o vivienda) que responde:

- ¿En qué año conviene vender para maximizar el retorno **real** (ya descontada la inflación)?
- ¿Cuánto tarda en duplicarse el down payment, en dólares nominales vs. poder adquisitivo real?
- ¿Cuál es el cash flow de hoy, bruto y neto, tomando en cuenta múltiples unidades con distintos estados de renta?
- ¿Cuánto se está perdiendo por unidades vacías u ocupadas sin pagar ("costo de espera")?

## Uso

Abre `index.html` en cualquier navegador — es una sola página autocontenida (sin build, sin dependencias). Todos los cálculos se actualizan en tiempo real al mover los inputs.

### Secciones de entrada

1. **Propiedad** — precio de compra, closing costs, property tax, seguro, HOA.
2. **Préstamo** — down payment, tasa de interés, plazo.
3. **Uso y renta** — modo Renta / Vivienda, unidades de la propiedad (nombre, renta de mercado, estado: Pagando / Ocupada sin pagar / Vacía / Por rentar), reservas de vacancia y mantenimiento.
4. **Venta** — apreciación esperada, comisión de realtor, closing costs de venta.
5. **Inflación** — para calcular el retorno en poder adquisitivo real.

### Resultados

- Panel del año óptimo de venta (retorno real anualizado más alto), colapsable.
- Cash flow de hoy (bruto/neto) y alertas de renta no cobrada por unidad.
- Gráfica de retorno acumulado nominal vs. real, con los puntos de cruce del 100%.
- Gráfica de retorno real anualizado por año, con el año óptimo marcado.
- Tabla año por año (se extiende automáticamente más allá de 10 años si el óptimo cae después).

## Supuestos

El property tax se calcula como % fijo sobre el precio de compra; seguro y HOA se mantienen constantes; la proyección multi-año usa solo la renta real (unidades "Pagando"), no la potencial; no se modela impuesto sobre la renta ni sobre ganancia de capital al vender. Ver el texto de "Supuestos del modelo" al final de la propia calculadora para el detalle completo.
