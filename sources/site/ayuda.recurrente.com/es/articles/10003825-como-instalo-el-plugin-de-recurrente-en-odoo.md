# Source: https://ayuda.recurrente.com/es/articles/10003825-como-instalo-el-plugin-de-recurrente-en-odoo

# ¿Cómo instalo el plugin de Recurrente en Odoo?

10 de julio de 2025

Índice de contenidos

[Enlaces de descarga del plugin:](https://ayuda.recurrente.com/es/articles/10003825-como-instalo-el-plugin-de-recurrente-en-odoo#h_899f93cfef)

[Paso 1: Activar Modo Desarrollador](https://ayuda.recurrente.com/es/articles/10003825-como-instalo-el-plugin-de-recurrente-en-odoo#h_9f51200161)

[Paso 2: Carga del plugin a Aplicaciones](https://ayuda.recurrente.com/es/articles/10003825-como-instalo-el-plugin-de-recurrente-en-odoo#h_4de17c542c)

[Paso 3: Activar módulo de Recurrente](https://ayuda.recurrente.com/es/articles/10003825-como-instalo-el-plugin-de-recurrente-en-odoo#h_dd3267b13f)

[Paso 4: Activar Recurrente en módulo de Sitio Web](https://ayuda.recurrente.com/es/articles/10003825-como-instalo-el-plugin-de-recurrente-en-odoo#h_917435ce7d)

[Paso 5: Obtener llaves de Recurrente](https://ayuda.recurrente.com/es/articles/10003825-como-instalo-el-plugin-de-recurrente-en-odoo#h_1ef740c34a)

[Paso 6: Configurar Webhooks de Recurrente](https://ayuda.recurrente.com/es/articles/10003825-como-instalo-el-plugin-de-recurrente-en-odoo#h_a01df49a04)

[Paso 7: Colocar llaves de Recurrente en Odoo](https://ayuda.recurrente.com/es/articles/10003825-como-instalo-el-plugin-de-recurrente-en-odoo#h_7e3bbcf9d6)

[¡Listo!](https://ayuda.recurrente.com/es/articles/10003825-como-instalo-el-plugin-de-recurrente-en-odoo#h_2da8c95ff4)

🙏 Este plugin ha sido desarrollado y mantenido por la maravillosa gente de [TipiCode](https://codingtipi.com) y mejorado por la comunidad Open Source. Si necesitas ayuda para una integración avanzada o "custom" a tu ambiente de Odoo, te recomendamos ponerte en contacto con [TipiCode](https://codingtipi.com/contact#info).

🔔 Antes de empezar con la instalación, asegúrate de ya haber creado tu cuenta de Recurrente. Vas a necesitar las "Llaves de API" y "Webhooks", que puedes accesar únicamente desde la sección de configuración de tu cuenta.

## Enlaces de descarga del plugin:

- [Plugin de Recurrente para Odoo 15.0](https://tipi-pod.sfo3.cdn.digitaloceanspaces.com/odoo/recurrente/Odoo-Recurrente-15.0.zip)

- [Plugin de Recurrente para Odoo 16.0](https://tipi-pod.sfo3.cdn.digitaloceanspaces.com/odoo/recurrente/Odoo-Recurrente-16.0.zip)

- [Plugin de Recurrente para Odoo 17.0](https://tipi-pod.sfo3.cdn.digitaloceanspaces.com/odoo/recurrente/Odoo-Recurrente-17.0.zip)

- [Plugin de Recurrente para Odoo 18.0](https://github.com/TipiCode/Odoo-Recurrente/tree/18.0)

## Paso 1: Activar Modo Desarrollador

Para iniciar necesitarás contar con el modo Desarrollador activado en Odoo. Para esto, dirígete a los Ajustes de Odoo y luego baja hasta donde encuentres la opción **Herramientas de Desarrollador** y presionaras donde dice **Activar Modo Desarrollador**. 
​

[![](https://downloads.intercomcdn.com/i/o/q0how4fq/1226359591/995ecf3375d5450203e2b09beb15/odoo-paso-1.jpeg?expires=1784052900&signature=d07f8d0429e8cb947220fcff7a160559e1f9c27418ebb0a06b22ea97960dbf23&req=dSIlEMp7lIRWWPMW1HO4zYoDfaaoN0ddpkcXKQNGtrc4d6ZySCQ%2BXtRqC6bE%0AgwUtyHcAckd4TYl%2BQXI%3D%0A)](https://downloads.intercomcdn.com/i/o/q0how4fq/1226359591/995ecf3375d5450203e2b09beb15/odoo-paso-1.jpeg?expires=1784052900&signature=d07f8d0429e8cb947220fcff7a160559e1f9c27418ebb0a06b22ea97960dbf23&req=dSIlEMp7lIRWWPMW1HO4zYoDfaaoN0ddpkcXKQNGtrc4d6ZySCQ%2BXtRqC6bE%0AgwUtyHcAckd4TYl%2BQXI%3D%0A)

## Paso 2: Carga del plugin a Aplicaciones

Descarga el plugin para tu versión de Odoo en los enlaces que se encuentran al inicio de este documento. Una vez descargado el plugin/módulo, cárgalo dentro de las aplicaciones de Odoo y presionas la opción de Actualizar lista de aplicaciones.

[![](https://downloads.intercomcdn.com/i/o/q0how4fq/1226363792/adac3ba6595e04ceec3ca33ae5ab/odoo-paso-2.jpeg?expires=1784052900&signature=9af40fa604884ae87bb4e521591e46b4aa212808738167012a4b8582c24bcee6&req=dSIlEMp4noZWW%2FMW1HO4zX3jyLEGV3DDk69tCaEfW14zNlw%2FIxXcd0rQHx2o%0A6t7NQ7jNmmkBKDNmEx0%3D%0A)](https://downloads.intercomcdn.com/i/o/q0how4fq/1226363792/adac3ba6595e04ceec3ca33ae5ab/odoo-paso-2.jpeg?expires=1784052900&signature=9af40fa604884ae87bb4e521591e46b4aa212808738167012a4b8582c24bcee6&req=dSIlEMp4noZWW%2FMW1HO4zX3jyLEGV3DDk69tCaEfW14zNlw%2FIxXcd0rQHx2o%0A6t7NQ7jNmmkBKDNmEx0%3D%0A)

## Paso 3: Activar módulo de Recurrente

Busca el módulo de Recurrente en tus aplicaciones y presiona la opción de Activar.

[![](https://downloads.intercomcdn.com/i/o/q0how4fq/1226370605/3664df535bc0c24e41df98ad79aa/odoo-pas-3.jpeg?expires=1784052900&signature=b4100aff82e94ac0e2047661e1300f0707ba98932844bd75b04ce1e2b1e818a6&req=dSIlEMp5nYdfXPMW1HO4zaOAHYnOgeRe%2FXH6C47Urj6EDQFl%2Fn0FYCSF2%2B2k%0Ay%2F5iMcXEryiL1Iq%2F2mM%3D%0A)](https://downloads.intercomcdn.com/i/o/q0how4fq/1226370605/3664df535bc0c24e41df98ad79aa/odoo-pas-3.jpeg?expires=1784052900&signature=b4100aff82e94ac0e2047661e1300f0707ba98932844bd75b04ce1e2b1e818a6&req=dSIlEMp5nYdfXPMW1HO4zaOAHYnOgeRe%2FXH6C47Urj6EDQFl%2Fn0FYCSF2%2B2k%0Ay%2F5iMcXEryiL1Iq%2F2mM%3D%0A)

## Paso 4: Activar Recurrente en módulo de Sitio Web

Luego de haber activado el módulo de Recurrente, dirígete al módulo de **Sitio Web** de Odoo. Dentro de las configuraciones presiona la opción de "Proveedores de pago", busca la opción de Recurrente y presiona Activar.

[![](https://downloads.intercomcdn.com/i/o/q0how4fq/1226449173/d850ed9833fc464b021be0a33cf0/odoo-paso-4.jpeg?expires=1784052900&signature=e2fb63be4319c5fcf376d5ec89a189d6c05e8ee28770d59ba1d303512e1ba920&req=dSIlEM16lIBYWvMW1HO4zT9OKyEqzwdbn6FhOec7obZR7fkMEWlQxTlZFhoo%0AK7kq%2Bs0cgwj4jLkOxEw%3D%0A)](https://downloads.intercomcdn.com/i/o/q0how4fq/1226449173/d850ed9833fc464b021be0a33cf0/odoo-paso-4.jpeg?expires=1784052900&signature=e2fb63be4319c5fcf376d5ec89a189d6c05e8ee28770d59ba1d303512e1ba920&req=dSIlEM16lIBYWvMW1HO4zT9OKyEqzwdbn6FhOec7obZR7fkMEWlQxTlZFhoo%0AK7kq%2Bs0cgwj4jLkOxEw%3D%0A)

## Paso 5: Obtener llaves de Recurrente

Ahora debes obtener tus llaves de Recurrente para poder configurar el módulo en Odoo. Ingresa a tu cuenta de Recurrente y dirígete a la opción de Mi Cuenta / Desarrolladores Y API.

[![](https://downloads.intercomcdn.com/i/o/q0how4fq/1226453156/88ccc85f2b52412416855c2391d7/llaves-recurrente.png?expires=1784052900&signature=f7e91eb30f5789204929cb12d4429bc0f29df4b75b16cb8e002fa3ef6ba2e9b2&req=dSIlEM17noBaX%2FMW1HO4zS4Nh%2BwG4Wxf1Szu4kzHXdEW2Dvp%2FLjyUbGJk05b%0AWzTIiGQ8LQyqoFb9q70%3D%0A)](https://downloads.intercomcdn.com/i/o/q0how4fq/1226453156/88ccc85f2b52412416855c2391d7/llaves-recurrente.png?expires=1784052900&signature=f7e91eb30f5789204929cb12d4429bc0f29df4b75b16cb8e002fa3ef6ba2e9b2&req=dSIlEM17noBaX%2FMW1HO4zS4Nh%2BwG4Wxf1Szu4kzHXdEW2Dvp%2FLjyUbGJk05b%0AWzTIiGQ8LQyqoFb9q70%3D%0A)

## Paso 6: Configurar Webhooks de Recurrente

Presiona el botón que dice Webhooks.

[![](https://downloads.intercomcdn.com/i/o/q0how4fq/1226459523/5dd8ba55cbf452c9e74626f83c7e/webhook.png?expires=1784052900&signature=0e45a3956b884cfe208597e2284f103fbc10e008a65e51712d06c70b41354aa6&req=dSIlEM17lIRdWvMW1HO4zWQken0OfxymY72e9XJo%2B2IZa8LhnoxHIl7GJuVW%0AveSxbXMUSMVR06svcao%3D%0A)](https://downloads.intercomcdn.com/i/o/q0how4fq/1226459523/5dd8ba55cbf452c9e74626f83c7e/webhook.png?expires=1784052900&signature=0e45a3956b884cfe208597e2284f103fbc10e008a65e51712d06c70b41354aa6&req=dSIlEM17lIRdWvMW1HO4zWQken0OfxymY72e9XJo%2B2IZa8LhnoxHIl7GJuVW%0AveSxbXMUSMVR06svcao%3D%0A)

Al presionar esta opción, el navegador te redirigirá a una plataforma llamada Svix. Selecciona la opción titulada Add Endpoint en la esquina superior derecha.

[![](https://downloads.intercomcdn.com/i/o/q0how4fq/1226463288/b7fa57a8309cd320ce31aca278f1/svix%2Bpaso%2B1.png?expires=1784052900&signature=7e4b9b3dc52742e475882c4375fef9091975cf1fc965d6d7d9ea84b39de8412f&req=dSIlEM14noNXUfMW1HO4zbP245dWmKSExyG%2BMQ7Qp9ZM1hk8EB2APbPOK37N%0A4T4wvK7%2BVMemmDwpfPc%3D%0A)](https://downloads.intercomcdn.com/i/o/q0how4fq/1226463288/b7fa57a8309cd320ce31aca278f1/svix%2Bpaso%2B1.png?expires=1784052900&signature=7e4b9b3dc52742e475882c4375fef9091975cf1fc965d6d7d9ea84b39de8412f&req=dSIlEM14noNXUfMW1HO4zbP245dWmKSExyG%2BMQ7Qp9ZM1hk8EB2APbPOK37N%0A4T4wvK7%2BVMemmDwpfPc%3D%0A)

En el campo de **“Endpoint URL”** coloca el dominio de tu sitio web seguido de **/payment/recurrente/webhook** , por ejemplo: **[https://midominio.com/payment/recurrente/webhook](https://midominio.com/payment/recurrente/webhook)**

[![](https://downloads.intercomcdn.com/i/o/q0how4fq/1226465908/ca0bb49d42ae70aa519f6e1ea833/svix-odoo.png?expires=1784052900&signature=9cc044206232c5dc02268e4d93d47fe363155d95ccf930a9b3425fb4809ce129&req=dSIlEM14mIhfUfMW1HO4zS6i%2FfIESBoltElsSB6MxmEuJstAxm0OgIb8sYSF%0A66vcx9fRw9OgxVk%2BAns%3D%0A)](https://downloads.intercomcdn.com/i/o/q0how4fq/1226465908/ca0bb49d42ae70aa519f6e1ea833/svix-odoo.png?expires=1784052900&signature=9cc044206232c5dc02268e4d93d47fe363155d95ccf930a9b3425fb4809ce129&req=dSIlEM14mIhfUfMW1HO4zS6i%2FfIESBoltElsSB6MxmEuJstAxm0OgIb8sYSF%0A66vcx9fRw9OgxVk%2BAns%3D%0A)

Luego, presiona el botón de "Create".

## Paso 7: Colocar llaves de Recurrente en Odoo

Por último, copia tus llaves de Recurrente, para ingresarlas en Odoo.

[![](https://downloads.intercomcdn.com/i/o/q0how4fq/1226481020/44521522d2fd7e87854431c2d273/Llaves+recurrente.png?expires=1784052900&signature=56bcae0dfb68997e73e536197eba055a6dba36c96d0cf6dd62588ec43311f1b7&req=dSIlEM12nIFdWfMW1HO4zdu7w9d07ngGEPLNbYiyXuQn7kOvvhQ3GcZopDUQ%0AI403sLHmvNiCCzv3Img%3D%0A)](https://downloads.intercomcdn.com/i/o/q0how4fq/1226481020/44521522d2fd7e87854431c2d273/Llaves+recurrente.png?expires=1784052900&signature=56bcae0dfb68997e73e536197eba055a6dba36c96d0cf6dd62588ec43311f1b7&req=dSIlEM12nIFdWfMW1HO4zdu7w9d07ngGEPLNbYiyXuQn7kOvvhQ3GcZopDUQ%0AI403sLHmvNiCCzv3Img%3D%0A)

Regresa a Odoo y en tus proveedores de pago busca a Recurrente. Dentro de esta vista puedes colocar tus llaves de integración de Recurrente.

[![](https://downloads.intercomcdn.com/i/o/q0how4fq/1226481393/76f220cba85713a2f0cf07acde3a/odoo-paso-5.jpeg?expires=1784052900&signature=4d73dca58aff4834a4c800c6e7d2ae133fe2bf750dbe7ce49f62cee7df5a87dc&req=dSIlEM12nIJWWvMW1HO4zSHUzMhynGPQZZ1NCgouYLzU1J4AgTvYe7NHht2t%0Athngfa3jYD0DrmF9XoE%3D%0A)](https://downloads.intercomcdn.com/i/o/q0how4fq/1226481393/76f220cba85713a2f0cf07acde3a/odoo-paso-5.jpeg?expires=1784052900&signature=4d73dca58aff4834a4c800c6e7d2ae133fe2bf750dbe7ce49f62cee7df5a87dc&req=dSIlEM12nIJWWvMW1HO4zSHUzMhynGPQZZ1NCgouYLzU1J4AgTvYe7NHht2t%0Athngfa3jYD0DrmF9XoE%3D%0A)

## **¡Listo!**

Tu instancia de Odoo ya está configurada para recibir pagos con tarjeta de Crédito/Debito utilizando Recurrente. Puedes aceptar pagos con tu sitio web de Odoo y/o generar links de pago automáticos para tus cotizaciones.

---

Artículos relacionados

- [¿Cómo realizo una transferencia de fondos?](https://ayuda.recurrente.com/es/articles/5614139-como-realizo-una-transferencia-de-fondos)
- [¿Cómo integrar Recurrente con Bubble?](https://ayuda.recurrente.com/es/articles/6531403-como-integrar-recurrente-con-bubble)
- [¿Cómo instalo el plugin de Recurrente en WooCommerce?](https://ayuda.recurrente.com/es/articles/8971522-como-instalo-el-plugin-de-recurrente-en-woocommerce)
- [¿Cuál es el costo de usar mi cuenta comercial en Recurrente?](https://ayuda.recurrente.com/es/articles/14759295-cual-es-el-costo-de-usar-mi-cuenta-comercial-en-recurrente)

¿Ha quedado contestada tu pregunta?

😞😐😃

Índice de contenidos

[Enlaces de descarga del plugin:](https://ayuda.recurrente.com/es/articles/10003825-como-instalo-el-plugin-de-recurrente-en-odoo#h_899f93cfef)

[Paso 1: Activar Modo Desarrollador](https://ayuda.recurrente.com/es/articles/10003825-como-instalo-el-plugin-de-recurrente-en-odoo#h_9f51200161)

[Paso 2: Carga del plugin a Aplicaciones](https://ayuda.recurrente.com/es/articles/10003825-como-instalo-el-plugin-de-recurrente-en-odoo#h_4de17c542c)

[Paso 3: Activar módulo de Recurrente](https://ayuda.recurrente.com/es/articles/10003825-como-instalo-el-plugin-de-recurrente-en-odoo#h_dd3267b13f)

[Paso 4: Activar Recurrente en módulo de Sitio Web](https://ayuda.recurrente.com/es/articles/10003825-como-instalo-el-plugin-de-recurrente-en-odoo#h_917435ce7d)

[Paso 5: Obtener llaves de Recurrente](https://ayuda.recurrente.com/es/articles/10003825-como-instalo-el-plugin-de-recurrente-en-odoo#h_1ef740c34a)

[Paso 6: Configurar Webhooks de Recurrente](https://ayuda.recurrente.com/es/articles/10003825-como-instalo-el-plugin-de-recurrente-en-odoo#h_a01df49a04)

[Paso 7: Colocar llaves de Recurrente en Odoo](https://ayuda.recurrente.com/es/articles/10003825-como-instalo-el-plugin-de-recurrente-en-odoo#h_7e3bbcf9d6)

[¡Listo!](https://ayuda.recurrente.com/es/articles/10003825-como-instalo-el-plugin-de-recurrente-en-odoo#h_2da8c95ff4)