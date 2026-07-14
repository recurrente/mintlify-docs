# Source: https://ayuda.recurrente.com/es/articles/15570697-como-crear-links-de-pago-con-monto-y-moneda-en-el-url

# Cómo crear links de pago con monto y moneda en el URL

Aprende a crear links dinámicos de pago en Recurrente usando monto y moneda directamente en el URL.

Actualizado hace más de 3 semanas

Índice de contenidos

[Formato del link](https://ayuda.recurrente.com/es/articles/15570697-como-crear-links-de-pago-con-monto-y-moneda-en-el-url#h_e6723db0f7)

[Ejemplos](https://ayuda.recurrente.com/es/articles/15570697-como-crear-links-de-pago-con-monto-y-moneda-en-el-url#h_195afc1e7d)

[Cuándo usarlo](https://ayuda.recurrente.com/es/articles/15570697-como-crear-links-de-pago-con-monto-y-moneda-en-el-url#h_c832ef3d30)

[Cómo configurarlo en tu web](https://ayuda.recurrente.com/es/articles/15570697-como-crear-links-de-pago-con-monto-y-moneda-en-el-url#h_d0ff456a80)

[Ejemplo práctico](https://ayuda.recurrente.com/es/articles/15570697-como-crear-links-de-pago-con-monto-y-moneda-en-el-url#h_44295e7e38)

[Cuándo conviene usar la API en vez de este URL](https://ayuda.recurrente.com/es/articles/15570697-como-crear-links-de-pago-con-monto-y-moneda-en-el-url#h_55eb58769d)

[Nota para soporte](https://ayuda.recurrente.com/es/articles/15570697-como-crear-links-de-pago-con-monto-y-moneda-en-el-url#h_fbfec9128d)

Si necesitas cobrar montos distintos sin crear un link manual para cada producto, puedes construir un link de pago de Recurrente usando el monto y la moneda directamente en el URL.

# Formato del link

```
https://app.recurrente.com/s/{tu-cuenta}/pagar/{monto}/{moneda}
```

También puedes omitir la moneda si quieres usar la moneda predeterminada de la cuenta:

```
https://app.recurrente.com/s/{tu-cuenta}/pagar/{monto}
```

# Ejemplos

- Para cobrar USD 50: 
 ​`https://app.recurrente.com/s/{tu-cuenta}/pagar/50/USD`

- Para cobrar Q350: 
 ​`https://app.recurrente.com/s/{tu-cuenta}/pagar/350/GTQ`

# Cuándo usarlo

Esta opción funciona bien cuando tu sitio web ya sabe cuánto debe cobrar y en qué moneda. Por ejemplo, si cada producto tiene su propio precio, tu página puede armar el link dinámicamente y enviar al cliente al checkout seguro de Recurrente.

# Cómo configurarlo en tu web

1. Identifica el slug o identificador de tu cuenta en Recurrente.

2. Toma el monto del producto o servicio que quieres cobrar.

3. Define la moneda: `GTQ` o `USD`.

4. Construye el link con este formato: 
 ​`https://app.recurrente.com/s/{tu-cuenta}/pagar/{monto}/{moneda}`

5. Usa ese link en el botón de pago de tu sitio, por ejemplo: “Pagar ahora”.

# Ejemplo práctico

Si tu tienda vende un producto de USD 50, el botón puede enviar al cliente a:

```
https://app.recurrente.com/s/{tu-cuenta}/pagar/50/USD
```

Si vende un producto de Q350, puede enviarlo a:

```
https://app.recurrente.com/s/{tu-cuenta}/pagar/350/GTQ
```

# Cuándo conviene usar la API en vez de este URL

Usa la API de checkouts si necesitas algo más avanzado, por ejemplo:

- Guardar el nombre exacto del producto.

- Enviar número de orden o metadata interna.

- Cobrar varios ítems en un mismo checkout.

- Conciliar automáticamente los pagos con tu sistema.

- Crear flujos más personalizados desde tu backend.

Para cobros simples con monto y moneda variable, el link por URL suele ser suficiente.

# Nota para soporte

Antes de enviarlo al cliente, cambia `{tu-cuenta}` por el slug real de su cuenta de Recurrente y prueba un link con un monto pequeño o de ejemplo para confirmar que abre el checkout correcto.

---

Artículos relacionados

- [¿Cómo funciona cobrar a clientes fuera de Guatemala?](https://ayuda.recurrente.com/es/articles/6415519-como-funciona-cobrar-a-clientes-fuera-de-guatemala)
- [Retiros Inmediatos: recibe tus fondos en minutos](https://ayuda.recurrente.com/es/articles/14555242-retiros-inmediatos-recibe-tus-fondos-en-minutos)
- [Tipos de cobro: conoce tus opciones para cobrar en Recurrente](https://ayuda.recurrente.com/es/articles/14811902-tipos-de-cobro-conoce-tus-opciones-para-cobrar-en-recurrente)
- [Cómo crear un producto de suscripción en tu tienda en línea](https://ayuda.recurrente.com/es/articles/14811920-como-crear-un-producto-de-suscripcion-en-tu-tienda-en-linea)
- [Cómo pagar por transferencia bancaria](https://ayuda.recurrente.com/es/articles/15706068-como-pagar-por-transferencia-bancaria)

¿Ha quedado contestada tu pregunta?

😞😐😃

Índice de contenidos

[Formato del link](https://ayuda.recurrente.com/es/articles/15570697-como-crear-links-de-pago-con-monto-y-moneda-en-el-url#h_e6723db0f7)

[Ejemplos](https://ayuda.recurrente.com/es/articles/15570697-como-crear-links-de-pago-con-monto-y-moneda-en-el-url#h_195afc1e7d)

[Cuándo usarlo](https://ayuda.recurrente.com/es/articles/15570697-como-crear-links-de-pago-con-monto-y-moneda-en-el-url#h_c832ef3d30)

[Cómo configurarlo en tu web](https://ayuda.recurrente.com/es/articles/15570697-como-crear-links-de-pago-con-monto-y-moneda-en-el-url#h_d0ff456a80)

[Ejemplo práctico](https://ayuda.recurrente.com/es/articles/15570697-como-crear-links-de-pago-con-monto-y-moneda-en-el-url#h_44295e7e38)

[Cuándo conviene usar la API en vez de este URL](https://ayuda.recurrente.com/es/articles/15570697-como-crear-links-de-pago-con-monto-y-moneda-en-el-url#h_55eb58769d)

[Nota para soporte](https://ayuda.recurrente.com/es/articles/15570697-como-crear-links-de-pago-con-monto-y-moneda-en-el-url#h_fbfec9128d)