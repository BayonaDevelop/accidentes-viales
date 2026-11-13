### Siniestralidad vial en México (INEGI-ATUS, 2015 en adelante)

- Objetivo:\*\* identificar cuándo, dónde y bajo qué condiciones los accidentes de tránsito dejan víctimas, a partir de los datos abiertos del INEGI.
- Mi rol:\*\* proyecto individual; definí el problema y el alcance, construí el proceso reproducible de descarga y limpieza en Python, hice el análisis exploratorio, ajusté un modelo de regresión logística con validación temporal y comuniqué los hallazgos.
- Fuente de los datos:\*\* INEGI. Estadística de Accidentes de Tránsito Terrestre en Zonas Urbanas y Suburbanas (ATUS). <https://www.inegi.org.mx/programas/accidentes/>

### Resultados principales (2015–2023)

- Se analizaron **3,238,288 accidentes** con **813,356 personas heridas** y **40,154 fallecidas**; el 19.0% de los accidentes dejó víctimas.
- Entre 2015 y 2023 los accidentes variaron -0.3%, las personas heridas -15.6% y las fallecidas +3.6%.
- El mayor volumen ocurre el **sábado a las 14 h**, pero la mayor proporción de accidentes con víctimas se da el **domingo a las 19 h** (26%).
- El tipo más frecuente es *colisión con vehículo automotor* (63% del total); el que más víctimas deja es *caída de pasajero* (100% con víctimas).
- La participación de motocicletas pasó de 10.8% a 19.5% de los accidentes; 50% de los accidentes con moto dejan víctimas frente a 14% del resto.
- Con aliento alcohólico, 28% de los accidentes deja víctimas (sin aliento: 18%); sin cinturón, 22% (con cinturón: 14%).
- **Sinaloa** tiene la mayor proporción de accidentes con víctimas (49%) y **Nuevo León** la menor (7%).
- El modelo logístico, evaluado en 2023 (año no visto), obtiene **ROC AUC = 0.83**. Controlando por los demás factores, los más asociados con víctimas son: TIPACCID_Colisión con peatón (atropellamiento) (45146.6×); TIPACCID_Caída de pasajero (1725.7×); TIPACCID_Colisión con ciclista (17.3×).
