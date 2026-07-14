# Source: https://ayuda.recurrente.com/es/articles/6531403-como-integrar-recurrente-con-bubble

# ¿Cómo integrar Recurrente con Bubble?

Guía de integración para la plataforma Bubble.

29 de enero de 2025

Índice de contenidos

[IMPORTANTE: Luego de inicializar, editar el endpoint y quitarle /initialize](https://ayuda.recurrente.com/es/articles/6531403-como-integrar-recurrente-con-bubble#h_0c3196cb14)

[Event Types](https://ayuda.recurrente.com/es/articles/6531403-como-integrar-recurrente-con-bubble#h_4587ec8b47)

En esta guía vamos a hacer un flow de checkout de Recurrente usando Bubble. 
​ 
Paso 1: Crea un plugin de API Connector hacia Recurrente 
​ 
Desde API Connector, haz click en Add Another API 
​ 
​

[![](https://downloads.intercomcdn.com/i/o/575454776/7340bc9405583e6a347ad1ec/1.png?expires=1784052900&signature=1bb8e4cfe6f411be63b1b3786c5d3c583edfa6bf8a29804fdae9840aa35e1d74&req=cSciEsx6moZZFb4f3HP0gFIZEOiq10HFBUOGYqDxdGrxeNfMinpBx8GYuHb%2F%0AruJgymSQnFSoTliq8Q%3D%3D%0A)](https://downloads.intercomcdn.com/i/o/575454776/7340bc9405583e6a347ad1ec/1.png?expires=1784052900&signature=1bb8e4cfe6f411be63b1b3786c5d3c583edfa6bf8a29804fdae9840aa35e1d74&req=cSciEsx6moZZFb4f3HP0gFIZEOiq10HFBUOGYqDxdGrxeNfMinpBx8GYuHb%2F%0AruJgymSQnFSoTliq8Q%3D%3D%0A)

Para sacar tus keys, ve a configuración: 
​ 
​

[![](https://downloads.intercomcdn.com/i/o/575454648/b61a44a236260918189d746b/2.png?expires=1784052900&signature=fb74a690cf4a29e52204577244cbf30ad7fa256850112564309f62fe5f48f3eb&req=cSciEsx6m4VXFb4f3HP0gLS%2BmMojnPGOnO0JMWvsx1Fz6CpzdMLuo27i1jxK%0AOQr1A6VlZBqX8qX3oQ%3D%3D%0A)](https://downloads.intercomcdn.com/i/o/575454648/b61a44a236260918189d746b/2.png?expires=1784052900&signature=fb74a690cf4a29e52204577244cbf30ad7fa256850112564309f62fe5f48f3eb&req=cSciEsx6m4VXFb4f3HP0gLS%2BmMojnPGOnO0JMWvsx1Fz6CpzdMLuo27i1jxK%0AOQr1A6VlZBqX8qX3oQ%3D%3D%0A)

Llena los datos de la siguiente manera:

[![](https://downloads.intercomcdn.com/i/o/575454304/80ce33a17baa57c89780a7d2/3.png?expires=1784052900&signature=d1e42fd73c55f11112c1abbd8a32c2bd4ad7652d9a5ec4a9bf550b6b6f94a083&req=cSciEsx6noFbFb4f3HP0gBnRmp%2BA77MbuefrME0iiW8WYeAO9VSwkyE1duEH%0A5juGpWV%2BWnC4EjxfbA%3D%3D%0A)](https://downloads.intercomcdn.com/i/o/575454304/80ce33a17baa57c89780a7d2/3.png?expires=1784052900&signature=d1e42fd73c55f11112c1abbd8a32c2bd4ad7652d9a5ec4a9bf550b6b6f94a083&req=cSciEsx6noFbFb4f3HP0gBnRmp%2BA77MbuefrME0iiW8WYeAO9VSwkyE1duEH%0A5juGpWV%2BWnC4EjxfbA%3D%3D%0A)

​

[![](https://downloads.intercomcdn.com/i/o/575454197/943e67b99a63280e1d6c06a2/4.png?expires=1784052900&signature=bf843e1d53ea1e99fdbfb2b8aaf429b810c541b53d2c0c317880947d872cc834&req=cSciEsx6nIhYFb4f3HP0gF7%2FqhRrgnde%2FKaULPS6AW3tG5bylig5BHQ8EMwg%0AFbCSnrp9Gf%2FK0%2B8dag%3D%3D%0A)](https://downloads.intercomcdn.com/i/o/575454197/943e67b99a63280e1d6c06a2/4.png?expires=1784052900&signature=bf843e1d53ea1e99fdbfb2b8aaf429b810c541b53d2c0c317880947d872cc834&req=cSciEsx6nIhYFb4f3HP0gF7%2FqhRrgnde%2FKaULPS6AW3tG5bylig5BHQ8EMwg%0AFbCSnrp9Gf%2FK0%2B8dag%3D%3D%0A)

```
{ "items": [{ "price_id": "<priceId>" }] }
```

Paso 2: Crear un Checkout al hacer click en un botón 
​ 
Crea un botón en tu página que diga "Pagar ahora"

[![](https://downloads.intercomcdn.com/i/o/575453806/2049794378c12682c7fdf995/5.png?expires=1784052900&signature=63ea0e5c96045867aef141033566ce9b1666bac5390a4475f1c7c40e4a2cc4b8&req=cSciEsx9lYFZFb4f3HP0gBC03KHvuPUMjuTY9Z4UDQXRUMxxtDfe8yVexzET%0At5ly%2B2NPRy3huEaNPA%3D%3D%0A)](https://downloads.intercomcdn.com/i/o/575453806/2049794378c12682c7fdf995/5.png?expires=1784052900&signature=63ea0e5c96045867aef141033566ce9b1666bac5390a4475f1c7c40e4a2cc4b8&req=cSciEsx9lYFZFb4f3HP0gBC03KHvuPUMjuTY9Z4UDQXRUMxxtDfe8yVexzET%0At5ly%2B2NPRy3huEaNPA%3D%3D%0A)

En caso necesiten user: 
​

[![](https://downloads.intercomcdn.com/i/o/575453231/954c089499672f36b8650593/6.png?expires=1784052900&signature=86019d05b566ef333cbe73a29b1482690264868787189a620a80717dda087842&req=cSciEsx9n4JeFb4f3HP0gOe5R%2BhKIw4orGa%2FzoyZW6X7yoojejSCmmCDB9Lb%0AJ4wUu9NhzerjMVYsIg%3D%3D%0A)](https://downloads.intercomcdn.com/i/o/575453231/954c089499672f36b8650593/6.png?expires=1784052900&signature=86019d05b566ef333cbe73a29b1482690264868787189a620a80717dda087842&req=cSciEsx9n4JeFb4f3HP0gOe5R%2BhKIw4orGa%2FzoyZW6X7yoojejSCmmCDB9Lb%0AJ4wUu9NhzerjMVYsIg%3D%3D%0A)

​ 
Paso 3: Webhooks 
​ 
Click en Webhook Dashboard 
​

[![](https://downloads.intercomcdn.com/i/o/575452940/19438cdc971cb6ab06eef523/7.png?expires=1784052900&signature=f6dca95f8880a7125235c1e7e9cc0d2ddda121312b57c53bf02f9cfb8a748c30&req=cSciEsx8lIVfFb4f3HP0gMwnjyPbQTmV2Ib4tkYRBsG1uFKU34Ze1CsFkKK0%0AVRXBdlrve8aP2TgLUg%3D%3D%0A)](https://downloads.intercomcdn.com/i/o/575452940/19438cdc971cb6ab06eef523/7.png?expires=1784052900&signature=f6dca95f8880a7125235c1e7e9cc0d2ddda121312b57c53bf02f9cfb8a748c30&req=cSciEsx8lIVfFb4f3HP0gMwnjyPbQTmV2Ib4tkYRBsG1uFKU34Ze1CsFkKK0%0AVRXBdlrve8aP2TgLUg%3D%3D%0A)

​ 
Click en Add Endpoint

[![](https://downloads.intercomcdn.com/i/o/575451668/fdcd3f2b54b83ae1e20a643b/8.png?expires=1784052900&signature=64f1515e7c6ea2149316eddc5117d30cfc0e06229dd1c7a7a500421c79cb590e&req=cSciEsx%2Fm4dXFb4f3HP0gBfq%2Fzgpv833u52Hy1tCDvJOgWAHYT1hn3MJdhGW%0A3Rs4EaxbVPcxtFkT8w%3D%3D%0A)](https://downloads.intercomcdn.com/i/o/575451668/fdcd3f2b54b83ae1e20a643b/8.png?expires=1784052900&signature=64f1515e7c6ea2149316eddc5117d30cfc0e06229dd1c7a7a500421c79cb590e&req=cSciEsx%2Fm4dXFb4f3HP0gBfq%2Fzgpv833u52Hy1tCDvJOgWAHYT1hn3MJdhGW%0A3Rs4EaxbVPcxtFkT8w%3D%3D%0A)

​ 
​ 
Ir a backend workflows:

[![](https://downloads.intercomcdn.com/i/o/575451456/dc8aca1e10c32a8488eac6f3/9.png?expires=1784052900&signature=cfe2e1ebeb6662239a58b893bc43ff7aec498aebc1ccb02cb86a3799fb84aba3&req=cSciEsx%2FmYRZFb4f3HP0gKPLu76gKJZcwUomcBEpXKVzJNL6VtvpwS%2FPu3zx%0Al6zKy4NXBY90TdMRTg%3D%3D%0A)](https://downloads.intercomcdn.com/i/o/575451456/dc8aca1e10c32a8488eac6f3/9.png?expires=1784052900&signature=cfe2e1ebeb6662239a58b893bc43ff7aec498aebc1ccb02cb86a3799fb84aba3&req=cSciEsx%2FmYRZFb4f3HP0gKPLu76gKJZcwUomcBEpXKVzJNL6VtvpwS%2FPu3zx%0Al6zKy4NXBY90TdMRTg%3D%3D%0A)

​ 
Crear un workflow nuevo: 
​ 
​

[![](https://downloads.intercomcdn.com/i/o/575451285/1b6e2ea53a50e873cb3e28e3/10.png?expires=1784052900&signature=c168bdbf05835abf1bbcd2d9c39843791deefbb2447bfa5e6bb4bfe6343e18f1&req=cSciEsx%2Fn4laFb4f3HP0gCPDdHF20AWpWluSECo8AZvA4ei0y4E%2BDvzn0tKv%0AP9gpryWetY5tVisJiQ%3D%3D%0A)](https://downloads.intercomcdn.com/i/o/575451285/1b6e2ea53a50e873cb3e28e3/10.png?expires=1784052900&signature=c168bdbf05835abf1bbcd2d9c39843791deefbb2447bfa5e6bb4bfe6343e18f1&req=cSciEsx%2Fn4laFb4f3HP0gCPDdHF20AWpWluSECo8AZvA4ei0y4E%2BDvzn0tKv%0AP9gpryWetY5tVisJiQ%3D%3D%0A)

​ 
Endpoint URL:

[![](https://downloads.intercomcdn.com/i/o/575451126/9b6ccd582baa5ea3f6896412/11.png?expires=1784052900&signature=8134602545c94bffefd12ad231beb3c65127c26b228cd5655358ded10a5342f2&req=cSciEsx%2FnINZFb4f3HP0gDkVxeh0QUJv1NTxU0gYcPsvkJcF2e5UtlBNeitV%0Aita%2BRHKgH1DGuiPFgg%3D%3D%0A)](https://downloads.intercomcdn.com/i/o/575451126/9b6ccd582baa5ea3f6896412/11.png?expires=1784052900&signature=8134602545c94bffefd12ad231beb3c65127c26b228cd5655358ded10a5342f2&req=cSciEsx%2FnINZFb4f3HP0gDkVxeh0QUJv1NTxU0gYcPsvkJcF2e5UtlBNeitV%0Aita%2BRHKgH1DGuiPFgg%3D%3D%0A)

​ 
​

# **IMPORTANTE: Luego de inicializar, editar el endpoint y quitarle /initialize**

[![](https://downloads.intercomcdn.com/i/o/575450265/5a87527e47a6735dfa7e9d30/12.png?expires=1784052900&signature=3a2f00bf542d515c154a6f0521a87af89285861c304e69700d496e7f6203b6b0&req=cSciEsx%2Bn4daFb4f3HP0gLHgGwUvdYbZ3dye1lCp6ZaeHOunjbDXRJfIdUGC%0AIY3Opy4lRJ0qEMOBbg%3D%3D%0A)](https://downloads.intercomcdn.com/i/o/575450265/5a87527e47a6735dfa7e9d30/12.png?expires=1784052900&signature=3a2f00bf542d515c154a6f0521a87af89285861c304e69700d496e7f6203b6b0&req=cSciEsx%2Bn4daFb4f3HP0gLHgGwUvdYbZ3dye1lCp6ZaeHOunjbDXRJfIdUGC%0AIY3Opy4lRJ0qEMOBbg%3D%3D%0A)

​ 
Cambiar created\_at a type = date 
​ 
​

# Event Types

```
payment_intent.succeeded payment_intent.failed subscription.create subscription.past_due subscription.cancel
```

​ 
Hacer las acciones correspondientes a cada event\_type:

[![](https://downloads.intercomcdn.com/i/o/575450105/9b787bba62eb0c195db0715c/13.png?expires=1784052900&signature=23a12c277770fa30fac1fb167002c6ebb793123aeec6f17ebb9b9640f6762089&req=cSciEsx%2BnIFaFb4f3HP0gLWqyuOQAMzgBW3%2FjzMTIq3Wt7GqfA5CHB3Ocm2S%0AVOE9pI1r8Q3FLp%2F%2B9g%3D%3D%0A)](https://downloads.intercomcdn.com/i/o/575450105/9b787bba62eb0c195db0715c/13.png?expires=1784052900&signature=23a12c277770fa30fac1fb167002c6ebb793123aeec6f17ebb9b9640f6762089&req=cSciEsx%2BnIFaFb4f3HP0gLWqyuOQAMzgBW3%2FjzMTIq3Wt7GqfA5CHB3Ocm2S%0AVOE9pI1r8Q3FLp%2F%2B9g%3D%3D%0A)

​

---

Artículos relacionados

- [¿Cómo instalo el plugin de Recurrente en WooCommerce?](https://ayuda.recurrente.com/es/articles/8971522-como-instalo-el-plugin-de-recurrente-en-woocommerce)
- [¿Cómo instalo el plugin de Recurrente en Odoo?](https://ayuda.recurrente.com/es/articles/10003825-como-instalo-el-plugin-de-recurrente-en-odoo)
- [¿Cómo crear y usar cupones de descuento en Recurrente?](https://ayuda.recurrente.com/es/articles/12271054-como-crear-y-usar-cupones-de-descuento-en-recurrente)
- [Cómo habilitar la Factura Electrónica (FEL) y descargar tu Firma Electrónica desde la SAT](https://ayuda.recurrente.com/es/articles/14113202-como-habilitar-la-factura-electronica-fel-y-descargar-tu-firma-electronica-desde-la-sat)

¿Ha quedado contestada tu pregunta?

😞😐😃

Índice de contenidos

[IMPORTANTE: Luego de inicializar, editar el endpoint y quitarle /initialize](https://ayuda.recurrente.com/es/articles/6531403-como-integrar-recurrente-con-bubble#h_0c3196cb14)

[Event Types](https://ayuda.recurrente.com/es/articles/6531403-como-integrar-recurrente-con-bubble#h_4587ec8b47)