<div align="right">
    <img src="../logo_US.png" alt="Go4Surprise Logo" width="100">
</div>
<div align="center">

# Grupo 10 - Go4Surprise

## 10 - TCO

### Sprint 3

<img src="../logo_Go4Surprise.png" alt="Go4Surprise Logo" width="200">

</div>

**Made by:** Mario Astudillo, Virginia Mesa


### Integrantes
<div style="columns: 2; -webkit-columns: 2; -moz-columns: 2;">

- Mohamed Abouri  
- Mario Astudillo Fierro  
- María Barrancos Márquez  
- Rafael Cabello Ranea  
- Manuel Chica López  
- David Delgado Pallares  
- José Gonzalo Domínguez Moreno  
- Virginia Mesa Pérez  
- José Manuel Miret Martín  
- Alejandro Nicolade Bravo  
- Manuel Palacios Pineda  
- Pablo Rodríguez Sánchez  
- Rubén Romero Sánchez  
- Paula Sánchez Gómez  
- Ramón Vergara Garrido  

</div>

---

## **1. Introducción**

**Go4Surprise** es una plataforma digital que actúa como intermediaria entre usuarios y empresas de ocio, con el objetivo de combatir la indecisión a la hora de elegir planes y fomentar el descubrimiento de experiencias. A través de un sistema de reservas sorpresa con categorías configurables, ayudamos a nuestros usuarios a disfrutar de actividades únicas mientras generamos tráfico y nuevos clientes para los negocios de ocio locales.
## **2. Modelo de Negocio**

Identificamos las siguientes fuentes principales de ingresos:

### **2.1 Acuerdos Comerciales con Empresas**

Go4Surprise establece convenios con empresas de ocio, que ofrecen sus experiencias a precios preferenciales a cambio de aumentar su visibilidad y asegurar un volumen mínimo de clientes. Este modelo es beneficioso para ambas partes: las empresas reducen el riesgo comercial y nosotros accedemos a mejores márgenes para la venta de experiencias.

### **2.2 Comisiones por Reserva**

Cada vez que un usuario reserva una experiencia, la empresa de ocio paga una comisión a la plataforma. Esta comisión puede ser fija o variable, según la naturaleza del evento. Al tratarse de un modelo basado en resultados, las empresas lo perciben como una inversión más que como un coste fijo. Además, es un modelo escalable: a mayor volumen de reservas, mayores ingresos.

### **2.3 Ingresos por Descarte de Categorías**

Los usuarios tienen la posibilidad de descartar categorías que no desean recibir. El primer descarte es gratuito y los adicionales tienen un coste de 5 € cada uno. Aunque se trata de una fuente de ingresos secundaria, puede aportar una suma relevante si el volumen de usuarios es significativo.

## **3. Análisis de Mercado**

### **3.1 Segmento demográfico**

Nuestro público objetivo se sitúa entre los **18 y 35 años**, un rango de edad activo digitalmente, con interés en experiencias novedosas, juegos, sorpresas y planes sociales.

### **3.2 Ámbito geográfico**

La primera fase de Go4Surprise se enfoca en las **5 principales ciudades de España**: Madrid, Barcelona, Valencia, Sevilla y Bilbao. En conjunto, estas ciudades agrupan a aproximadamente **1.571.000 personas entre 18 y 35 años**.

## **4. Estimación de Costes**

En esta sección se detallan los costes necesarios para el desarrollo, lanzamiento y operación de la plataforma, diferenciando entre costes de inversión (**CAPEX**) y costes operativos mensuales (**OPEX**).

### **4.1 CAPEX (Costes de Inversión)**
| **Concepto**                 | **Detalle**                                                                                     | **Coste (€)**  |
|-----------------------------|--------------------------------------------------------------------------------------------------|----------------|
| **Dominio**                 | Registro IONOS (primer año)                                                                      | 1 €            |
| **Legalidad y Registro**    | Creación de empresa, asesoramiento legal, cumplimiento normativo (incl. RGPD)                    | 1.000 €        |
| **Infraestructura técnica inicial** | Google App Engine: 0,093 €/h × 24h × 70 días                                                 | 156,24 €       |
| **Desarrollo de la plataforma**     | Ver explicación detallada abajo                                                              | 61.810 €       |
| **Marketing de lanzamiento**       | Branding, diseño visual, vídeo promocional, primeras campañas en redes sociales, anuncios     | 3.000 €        |
**Total CAPEX:** **66.967,24 €**

### **Desarrollo de la Plataforma**

El desarrollo se llevó a cabo en una fase intensiva de 14 semanas, a cargo de un equipo técnico formado por:

- 8 desarrolladores frontend (React)
- 8 desarrolladores backend (Node.js, APIs, base de datos)

Cada miembro trabajó 10 horas semanales, con tarifas estándar para perfiles junior:

- Frontend: 20 €/h → 22.400 €
- Backend: 22 €/h → 24.640 €
- Total salarios brutos: 47.040 €

**Costes sociales estimados:**

- Contingencias Comunes: 23,60%
- Desempleo: 5,50%
- Formación Profesional: 0,60%
- FOGASA: 0,20%
- Accidentes de trabajo: 1,50%

**Total costes sociales:** 14.770 € (aprox. 31,40% del salario bruto)

**Coste total desarrollo (14 semanas): 61.810 €**

### **4.2 OPEX (Costes Operativos Mensuales)**
| **Concepto**                    | **Detalle**                                                                                             | **Coste (€/mes)** |
|--------------------------------|----------------------------------------------------------------------------------------------------------|-------------------|
| **Desarrollo y mantenimiento** | Mantenimiento, soporte técnico y evolución del software                                                  | 4.157 €           |
| **Mantenimiento técnico**      | Infraestructura y servidores (Google App Engine)                                                         | 94 €              |
| **Procesamiento de pagos**     | Comisiones de pasarela de pago (3% sobre volumen estimado de transacciones)                             | 600 €             |
| **Soporte al cliente**         | Atención parcial por agente + herramientas gratuitas (ej. Tidio/Crisp en fases iniciales)                | 960 €             |
| **Marketing mensual (opcional)** | Campañas de adquisición, redes sociales, anuncios pagados, colaboraciones con influencers, etc.         | Variable          |

**Total OPEX estimado:** **5.811 €/mes**

### **4.3 Resumen General de Costes**
| **Tipo de coste**                   | **Importe estimado** |
|-------------------------------------|-----------------------|
| **CAPEX total**                     | 66.967,24 €           |
| **OPEX mensual estimado**           | 5.811 €               |
| **Total inicial (CAPEX + 1 mes OPEX)** | 72.778,24 €           |

## **5. Estimación de Ingresos**

### **5.1 Supuestos Clave**

Para estimar el potencial de ingresos de Go4Surprise, se parte del análisis del mercado objetivo descrito previamente. De los aproximadamente **1.571.000 usuarios potenciales** (jóvenes entre 18 y 35 años en las principales cinco ciudades de España), se establecen tres escenarios de adopción de la plataforma:

- **Escenario pesimista**: 0,2% de adopción → **3.142 usuarios potenciales**
- **Escenario medio**: 0,5% de adopción → **7.855 usuarios potenciales**
- **Escenario optimista**: 1,0% de adopción → **15.710 usuarios potenciales**

Estas cifras suponen usuarios activos que realizarían al menos una reserva mensual, lo que permite proyectar los ingresos mensuales de la plataforma.

### **5.2 Ingresos Mensuales Estimados**

Las siguientes proyecciones de ingresos se basan en una serie de suposiciones clave:

- Comisión por reserva: **15%** del precio de la experiencia
- Precio medio por experiencia: **30 €**
- Ingreso medio por reserva: **4,5 €**
- Tarifa por descarte adicional: **5 €** (primer descarte gratuito)
- Porcentaje estimado de usuarios que descartan al menos una categoría adicional: **5%**
- Promedio de descartes por usuario que utiliza esta función: **2 descartes (10 € por usuario)**

Asumiendo que cada usuario realiza **1 reserva al mes**, se obtienen las siguientes estimaciones:
| **Escenario** | **Usuarios** | **Ingresos por reservas** | **Ingresos por descartes** | **Ingreso total mensual** |
|---------------|--------------|----------------------------|-----------------------------|----------------------------|
| **Pesimista** | 3.142        | 14.139 €                   | 1.571 €                     | 15.710 €                   |
| **Medio**     | 7.855        | 35.348 €                   | 3.927 €                     | 39.275 €                   |
| **Optimista** | 15.710       | 70.695 €                   | 7.855 €                     | 78.550 €                   |
