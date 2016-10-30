# PGPI - Tareas T5

> Francisco Javier Bolívar Lupiáñez

**Analice los distintos parámetros que permiten calibrar el modelo de estimación COCOMO II:**

![cocomoii](https://cloud.githubusercontent.com/assets/6973564/19835437/b24fa0c8-9e86-11e6-9118-63c27a927a35.png)

* **5 factores de escala [SF: scale factors]**
* **17 multiplicadores de esfuerzo [EM: effor multipliers]**

> **Sección 3 del manual de COCOMO II: http://csse.usc.edu/csse/research/COCOMOII/cocomo2000.0/CII_modelman2000.0.pdf**

> **COCOMO® II Cost Driver and Scale Driver Help: http://sunset.usc.edu/research/COCOMOII/expert_cocomo/drivers.html**

**Para proyectos del mismo tamaño (en KSLOC), compruebe el efecto que tiene el ajuste de dichos parámetros en diferentes escenarios. En particular, realice estimaciones para los siguientes proyectos:**

* **Aplicación web desarrollada por un equipo experimentado en el uso de las herramientas necesarias para el proyecto.**
* **Middleware de alto rendimiento para la construcción de sistemas distribuidos heterogéneos.**
* **Sistema empotrado para una plataforma hardware acutalmente en desarrollo (totalmente novedosa).**

**Elabore una tabla en la que se recojan los valores numéricos adecuados de los distintos parámetros para cada uno de los escenarios planteados:**

| Parámetro            | Web App  | Middleware  | Hardware  |
| -------------------- | -------- | ----------- | --------- |
| SF<sub>1</sub> PREC  | 1.24     | 2.48        | 6.20      |
| SF<sub>2</sub> FLEX  | 2.03     | 2.03        | 1.01      |
| SF<sub>3</sub> RESL  | 1.41     | 2.83        | 5.65      |
| SF<sub>4</sub> TEAM  | 1.10     | 2.19        | 3.29      |
| SF<sub>5</sub> PMAT  | 1.56     | 3.12        | 4.68      |
| **ΣSF<sub>j</sub>**  | **7.34** | **12.65**   | **20.83** |
| EM<sub>1</sub> RELY  | 1.00     | 1.00        | 1.00      |
| EM<sub>2</sub> DATA  | 1.28     | 0.90        | 0.90      |
| EM<sub>3</sub> CPLX  | 0.87     | 1.34        | 1.74      |
| EM<sub>4</sub> RUSE  | 1.00     | 1.07        | 1.07      |
| EM<sub>5</sub> DOCU  | 1.00     | 1.00        | 1.00      |
| EM<sub>6</sub> TIME  | 1.29     | 1.10        | 1.10      |
| EM<sub>7</sub> STOR  | 1.05     | 1.00        | 1.05      |
| EM<sub>8</sub> PVOL  | 0.87     | 1.15        | 1.30      |
| EM<sub>9</sub> ACAP  | 1.00     | 1.00        | 1.00      |
| EM<sub>10</sub> PCAP | 0.76     | 1.00        | 1.00      |
| EM<sub>11</sub> PCON | 0.90     | 0.90        | 0.90      |
| EM<sub>12</sub> APEX | 0.81     | 1.00        | 1.22      |
| EM<sub>13</sub> PLEX | 0.85     | 1.00        | 1.19      |
| EM<sub>14</sub> LTEX | 0.84     | 1.00        | 1.09      |
| EM<sub>15</sub> TOOL | 1.09     | 0.90        | 1.00      |
| EM<sub>16</sub> SITE | 0.86     | 0.93        | 1.09      |
| EM<sub>17</sub> SCED | 1.00     | 1.00        | 1.00      |
| **ΠEM<sub>i</sub>**  | **0.49** | **1.23**    | **3.91**  |

---

**Utilizando la expresión general del modelo COCOMO II:**

![cocomoii](https://cloud.githubusercontent.com/assets/6973564/19835437/b24fa0c8-9e86-11e6-9118-63c27a927a35.png)

**estime el esfuerzo necesario para desarrollar un proyecto de 10 KSLOC, 100 KSLOC y 1000 KSLOC en cada uno de los escenarios anteriores y rellene la siguiente tabla:**

| Tamaño      | Web App      | Middleware    | Hardware      |
| ----------- | ------------ | ------------- | ------------- |
| 10 KSLOC    | 13.87 p.m.   | 39.33 p.m.    | 150.95 p.m.   |
| 100 KSLOC   | 133.46 p.m.  | 427.81 p.m.   | 1982.09 p.m.  |
| 1000 KSLOC  | 1284.53 p.m. | 4653.21 p.m.  | 26027.00 p.m. |
