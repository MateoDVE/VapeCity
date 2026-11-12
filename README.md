# Vape City — Sistema de Catálogo Digital Neón y Gestión Administrativa

Plataforma integral de **Vape City (Cochabamba, Bolivia)** para la exhibición interactiva del catálogo de vaporizadores **WAKA** bajo la identidad visual **Grafiti Neón** y la administración completa de inventario por sabores, preparación de pedidos, reabastecimiento a distribuidor y control de ganancias reales.

---

## 📚 Índice de Documentación Oficial del Proyecto

Toda la documentación funcional, visual, comercial y técnica se encuentra en la carpeta [`Docs/`](file:///c:/Users/Mateo/Documents/Mateo%20Tareas/VapeCity/Docs):

1. **[`01_BRANDING_Y_DISENO_UI.md`](file:///c:/Users/Mateo/Documents/Mateo%20Tareas/VapeCity/Docs/01_BRANDING_Y_DISENO_UI.md)**
   - Guía de marca **Grafiti Neón (Versión 2)** extraída de [`Vape City Premium.html`](file:///c:/Users/Mateo/Documents/Mateo%20Tareas/VapeCity/Docs/Vape%20City%20Premium.html).
   - Paleta de colores oficial (`#0A0A0D` Asfalto, `#FF2E93` Rosa, `#19B8FF` Cian, `#9BE82B` Lima), tipografías (`Permanent Marker` + `Barlow Condensed`), reglas de brillo y componentes UI.
2. **[`02_CATALOGO_PRODUCTOS_Y_SABORES.md`](file:///c:/Users/Mateo/Documents/Mateo%20Tareas/VapeCity/Docs/02_CATALOGO_PRODUCTOS_Y_SABORES.md)**
   - Matriz maestra de productos WAKA (`Pocket 6K`, `Go 10K`, `Crystal 12K`, `Creator 20K Lego`, `Batería Lego`, `Apex 30K`, `Blast 36K`, `Icon 50K`, `Double 70K`).
   - Costos de distribuidor, precios de mercado, precios de venta catálogo, márgenes unitarios y listado completo de los 33+ sabores por línea.
3. **[`03_REGLAS_DE_NEGOCIO_E_INVENTARIO.md`](file:///c:/Users/Mateo/Documents/Mateo%20Tareas/VapeCity/Docs/03_REGLAS_DE_NEGOCIO_E_INVENTARIO.md)**
   - Reglas de control de inventario por variante de sabor y semáforo automático (`DISPONIBLE`, `BAJO STOCK`, `AGOTADO`).
   - Flujo de preparación de pedidos de clientes (`PENDIENTE` $\to$ `EN_PREPARACION` $\to$ `ENTREGADO_PAGADO` / `CANCELADO`).
   - Fórmulas contables para saber **cuánto tenemos vendido**, **cuánto estamos ganando** (Ganancia Real vs. Potencial) y el simulador de compras al distribuidor contra presupuesto.
4. **[`04_ARQUITECTURA_Y_MODELO_DE_DATOS.md`](file:///c:/Users/Mateo/Documents/Mateo%20Tareas/VapeCity/Docs/04_ARQUITECTURA_Y_MODELO_DE_DATOS.md)**
   - Arquitectura para [`FrontVapeCity`](file:///c:/Users/Mateo/Documents/Mateo%20Tareas/VapeCity/Vapecity/FrontVapeCity) (Angular 20) y [`back-vape-city`](file:///c:/Users/Mateo/Documents/Mateo%20Tareas/VapeCity/Vapecity/back-vape-city) (NestJS 11).
   - Diagrama Entidad-Relación (ERD), estructura de carpetas y especificación de endpoints REST.
5. **[`05_DISENO_BASE_DE_DATOS.md`](file:///c:/Users/Mateo/Documents/Mateo%20Tareas/VapeCity/Docs/05_DISENO_BASE_DE_DATOS.md)** y **[`schema_vapecity.sql`](file:///c:/Users/Mateo/Documents/Mateo%20Tareas/VapeCity/Docs/schema_vapecity.sql)**
   - Diseño físico de base de datos PostgreSQL / Supabase con tablas, tipos `ENUM`, columnas autocalculadas, triggers de negocio, vistas de Dashboard y seed completo de las 9 líneas WAKA y sus 37 sabores.

---

## 🛠️ Estructura del Repositorio

- [`Docs/`](file:///c:/Users/Mateo/Documents/Mateo%20Tareas/VapeCity/Docs): Documentación de negocio, manual de marca, catálogos PDF, hojas de cálculo base y recursos gráficos.
- [`Vapecity/FrontVapeCity/`](file:///c:/Users/Mateo/Documents/Mateo%20Tareas/VapeCity/Vapecity/FrontVapeCity): Aplicación Frontend en Angular 20 (Catálogo Público Neón + Panel Admin).
- [`Vapecity/back-vape-city/`](file:///c:/Users/Mateo/Documents/Mateo%20Tareas/VapeCity/Vapecity/back-vape-city): Servidor Backend en NestJS 11.
