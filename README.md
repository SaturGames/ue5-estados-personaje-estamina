# UE5 - Sistema Modular de Estados de Personaje, Estamina y Parkour | Gameplay Mechanics

Sistema modular y desacoplado de movimiento avanzado, gestión de estamina, validación de espacio libre (*headroom check*) y mecánicas de impulsión en entorno (*Launch Pad*) desarrollado en **Unreal Engine 5.4.4**. Diseñado enfocado en arquitectura limpia, escalabilidad y separación de responsabilidades lógicas mediante el uso de Eventos Personalizados (CE), transiciones de estado de personaje y gestión contextual de UI e Inputs.

> **Core Focus:** Clean Architecture, Character State Management, Headroom Validation, Movement Physics & Game Feel.

---

## Demostración Visual y Arquitectura de Blueprints

### Showcase del Prototipo (Greybox & Gameplay)
<img width="1929" height="991" alt="1G" src="https://github.com/user-attachments/assets/e39ce3d8-9b6e-4d6d-ad24-257a524345a7" />
<img width="1929" height="991" alt="2G" src="https://github.com/user-attachments/assets/64e564c2-9520-4c71-a22c-831898fbb0ce" />
<img width="1929" height="953" alt="3G" src="https://github.com/user-attachments/assets/2e338c2b-1321-4110-bef3-af82033aab97" />
<img width="1929" height="953" alt="4G" src="https://github.com/user-attachments/assets/aa2a6b67-fc30-4b04-8082-338ea7f14ea1" />

### Arquitectura de Blueprints y Código Documentado
<img width="1929" height="1050" alt="1E" src="https://github.com/user-attachments/assets/a2ae040e-34df-44de-b7f0-ce7c74879b44" />
<img width="1929" height="1050" alt="2E" src="https://github.com/user-attachments/assets/52b0e8fc-053b-4bb1-9c5a-109a4df6e349" />
<img width="1929" height="1050" alt="3E" src="https://github.com/user-attachments/assets/243775a4-eff4-409c-a042-a542d46898d6" />
<img width="1929" height="1050" alt="4E" src="https://github.com/user-attachments/assets/e94b0187-a002-4a88-b7e3-e5a8ce7b6f2d" />

---

## Aspectos Técnicos e Implementación

- **Gestión de Estados & Estamina:** Sistema de esprintar con consumo progresivo, regeneración automatizada y transición forzada a caminata al agotarse el recurso mediante el control estricto de banderas (*flags*).
- **Validación de Espacio Libre (Headroom Check):** Lógica de agachado (*Crouch/Crawl*) respaldada por volumetría de colisión (*Box Collision*) que restringe dinámicamente el cambio de postura si existe un obstáculo superior.
- **Trampolín de Impulso (Launch Pad):** Mecánica de rebotador mediante aplicación de vectores de fuerza (`Launch Character`) e integración de audio localizado en eventos de superposición de colisión (*Overlap*).
- **Flujo de Gameplay & UI:** Circuito interactivo con detección de meta (Punto A a Punto B), feedback sonoro de victoria e interfaz gráfica con gestión de entradas (`Restart` / `Quit`) configurada con pasarela de clics (`Not Testable / Hit Test Invisible`).
- **Game Feel & Feedback Audiovisual:** Integración de efectos de audio 2D y 3D en momentos clave de interacción para optimizar la respuesta táctil del jugador y la inmersión dentro del prototipo técnico.

---

## Demostración en Video

- **Prototipo Gameplay & Demo:** [Ver demostración en LinkedIn](https://www.linkedin.com/feed/update/urn:li:activity:7518771217731055616/)

---

**Desarrollado por Satur Games** | *Gameplay & Systems Programmer*
