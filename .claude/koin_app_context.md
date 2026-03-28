# Koin App — Documento de Contexto
> Uso interno · Equipo de Data & Marketing  
> Última actualización: marzo 2026

---

## 1. ¿Qué es Koin App?

Koin App es la aplicación mobile de Koin (Grupo Prosus) orientada al consumidor final en Brasil. Su propuesta de valor central es permitir compras en cuotas vía **Pix Parcelado**, sin necesidad de tarjeta de crédito. Está diseñada para un segmento que históricamente tiene acceso limitado al crédito formal: personas sin tarjeta, con límite bajo o con historial crediticio escaso.

---

## 2. Público objetivo

| Dimensión | Detalle |
|---|---|
| **Edad** | 20 a 55 años |
| **Clase social** | Principalmente C/D/E · algo de A/B |
| **Perfil crediticio** | Sin tarjeta de crédito, límite bajo, o en proceso de construcción de historial |
| **Geografía** | Cobertura nacional · Mayor concentración en SP, RJ, BA, MG, Brasília, PR y RS |

---

## 3. Producto core: Pix Parcelado

El usuario puede financiar compras en cuotas usando Pix, sin tarjeta. El acceso al producto está condicionado a la evaluación de crédito interna de Koin.

### Lógica de límite de crédito
- El límite inicial varía entre **R$200 y R$500**, según el resultado de la evaluación.
- A medida que el usuario compra y paga en tiempo, el límite **se restituye y puede incrementarse**.
- Sin límite aprobado, el usuario no puede realizar ninguna compra.

### Productos adicionales
Por ahora solo Pix Parcelado. No hay productos adicionales activos en la app.

---

## 4. Funnel del usuario

```
Install → Cadastro → Evaluación de crédito → Límite aprobado → Primera compra (Activación)
```

| Etapa | Descripción | Notas |
|---|---|---|
| **Install** | Descarga de la app | Puede venir de 4 orígenes distintos |
| **Cadastro** | Registro en la app | [TBD: ¿qué información/documentación se requiere?] |
| **Evaluación de crédito** | Score interno de Koin | ~35% de usuarios reciben límite · varía según origen del install · muchos campos pero baja fricción de documentación |
| **Sin límite** | Usuario registrado pero sin crédito disponible | No puede comprar · Sin estrategia de nurturing activa por ahora |
| **Con límite** | Usuario habilitado para comprar | Límite inicial R$200–R$500 |
| **Activación** ⭐ | **Primera compra realizada** | Evento de activación del negocio |
| **Recurrencia** | Segunda compra en adelante | Retención y crecimiento de límite |

> ⚠️ **El evento de activación es la primera compra, no el registro.**  
> Un usuario cadastrado sin compra no es considerado activo.

---

## 5. Canales de adquisición (Origens)

| Origen | Descripción |
|---|---|
| **Marketplaces de crédito** | Plataformas comparadoras / agregadoras de crédito donde Koin tiene presencia |
| **Mídia (Paid Ads)** | Campañas pagadas de performance (Meta, Google, etc.) |
| **Orgánico** | Descarga directa, boca a boca, ASO |
| **B2B** | Migración de usuarios de lojas con integración Koin en checkout hacia la app · Volumen bajo · Considerados usuarios de mayor calidad |

---

## 6. Lojas disponibles en la app

Los usuarios pueden comprar de dos formas dentro de la app:
- **Redirigido a lojas**: la app redirige al usuario a la cuenta del merchant.
- **Código Pix externo**: el usuario puede traer un código Pix generado desde cualquier tienda externa.

El **top 4 por volumen**:

1. Shopee
2. iFood
3. MercadoLibre
4. Amazon



---

## 7. Métricas clave del negocio

| Métrica | Descripción | Notas |
|---|---|---|
| **Activación** | % de installs que realizan su primera compra | KPI principal de conversión post-install |
| **GMV** | Volumen total transaccionado en la app | Principal indicador de salud del negocio |
| **CAC por canal** | Costo de adquisición por cliente activado, segmentado por origen | Clave para optimización de inversión en Mídia |
| **Retención / Recurrencia** | % de usuarios que realizan una segunda compra y más | Indicador de salud del producto y del portafolio de crédito |

---

## 8. Canales de comunicación con el usuario

Los canales activos para lifecycle y retención son **Email, Push notifications y WhatsApp**.

---

## 9. Competidores relevantes

| Competidor | Posicionamiento | Nota |
|---|---|---|
| **Pagaleve** | Principal competidor directo en BNPL Brasil | Opera solo B2B (checkout de merchants), sin canal B2C directo |
| **Jeitto** | BNPL para clases populares | Modelo diferente al de Koin App |
| **Neon Parcelado** | Parcelamento vinculado a cuenta digital Neon | |
| **Nubank Parcelado** | Parcelamento sin tarjeta de Nubank | |
| **Geru** | Crédito personal digital | |
| **Addi** | BNPL regional (mayor presencia en Colombia) | |

[TBD: ¿cuál es la diferenciación de Koin App frente a estos jugadores en la propuesta al usuario final?]

---

## 10. Pendientes / Placeholders

- [ ] Total de lojas activas en la app
- [ ] Diferenciación de Koin vs competidores en la propuesta al usuario final
- [ ] Tasa de activación (install → primera compra) por origen
