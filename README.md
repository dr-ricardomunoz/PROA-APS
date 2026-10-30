# PROA APS · Asistente clínico para ITU

Herramienta web estática, responsive y sin almacenamiento de datos, inspirada en el diseño institucional de las calculadoras de presión arterial infantil y edad corregida del CESFAM Dr. Mario Salcedo Sepúlveda.

## Funcionamiento
Se selecciona población, presentación clínica, criterios de gravedad, factores de riesgo, urocultivo, alergias, función renal y otras precauciones. El asistente entrega cuatro bloques: conducta inmediata, exámenes, tratamiento y seguimiento. Incluye cálculo orientativo de dosis por peso pediátrico, precauciones por semanas de gestación y botón para copiar orientación sin identificadores.

## Base documental
- Protocolo institucional *Tratamiento de infecciones del tracto urinario*, PROA ITU versión 01, aprobado agosto 2026, págs. 5 a 15.
- Contraste: EAU, *Urological Infections* (2026); ACOG, *Urinary Tract Infections in Pregnant Individuals* (2023); NICE NG109 y NG224.

## Estado de seguridad
**PILOTO – Validación clínica pendiente antes de uso asistencial general.**

Se han dejado sin prescripción automatizada las pautas de pielonefritis aguda ambulatoria, las situaciones con compromiso prostático y esquemas gestacionales/pediátricos que requieren revisión frente a guías externas. El equipo PROA/Farmacia debe validar las diferencias de duración y fármacos antes de difundir como herramienta institucional oficial.

La aplicación no solicita ni almacena RUT, nombres o identificadores. No tiene backend ni analítica.

## Pruebas
Ejecutar: node tests/clinical-scenarios.test.cjs

## Publicación
GitHub Pages en la rama principal, directorio raíz. El proyecto admite agregar módulos PROA futuros bajo carpetas independientes.
