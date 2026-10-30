# PROA APS · Asistente clínico para ITU

Herramienta web estática, responsive y sin almacenamiento de datos, inspirada en el diseño institucional de las calculadoras de presión arterial infantil y edad corregida del CESFAM Dr. Mario Salcedo Sepúlveda.

## Funcionamiento
Se selecciona población, presentación clínica, criterios de gravedad, factores de riesgo, urocultivo, alergias, función renal y otras precauciones. El asistente entrega cuatro bloques: conducta inmediata, exámenes, tratamiento y seguimiento. Incluye cálculo orientativo de dosis por peso pediátrico, precauciones por semanas de gestación y rutas específicas de prostatitis, sin ingresar datos identificatorios.

## Base documental
- Protocolo institucional *Tratamiento de infecciones del tracto urinario*, PROA ITU versión 01, aprobado agosto 2026, págs. 5 a 15.
- Contraste: EAU, *Urological Infections* (2026); ACOG, *Urinary Tract Infections in Pregnant Individuals* (2023); NICE NG109 y NG224.

## Estado de seguridad
**PILOTO – Validación clínica pendiente antes de uso asistencial general.**

Se mantienen sin prescripción automatizada las pautas de pielonefritis ambulatoria que requieren validación. En prostatitis aguda, el protocolo incluye ciprofloxacino 500 mg VO cada 12 h por 7–14 días y cotrimoxazol 160/800 mg VO cada 12 h por 14 días; la herramienta muestra ciprofloxacino como opción empírica **condicionada** con duración de 14 días, y cotrimoxazol como alternativa únicamente ante sensibilidad demostrada. Los esquemas deben ajustarse según antibiograma, resistencia, comorbilidades y tolerancia, con control a las 48 h. La disponibilidad real de los comprimidos debe verificarse con Farmacia local. No se proponen automáticamente cefalexina ni formulaciones pediátricas señaladas como no disponibles en APS. Equipo PROA/Farmacia debe validar diferencias y disponibilidad antes de la difusión institucional.

La aplicación no solicita ni almacena RUT, nombres o identificadores. No tiene backend ni analítica.

## Pruebas
Ejecutar: node tests/clinical-scenarios.test.cjs

## Publicación
GitHub Pages en la rama principal, directorio raíz. El proyecto admite agregar módulos PROA futuros bajo carpetas independientes.
