# VR_Robot Control System Axis 6 (Basico_Avanzado)
**Justifiacion tecnica:**

La presente investigación surge ante la necesidad de modernizar los métodos de enseñanza en la robótica industrial. A diferencia de los métodos tradicionales basados en el uso exclusivo de Teach Pendants físicos y lógica de PLC aislada, este proyecto implementa un Gemelo Digital Inmersivo. Mediante el uso de realidad virtual (VR) y el cumplimiento de normativas de seguridad funcional como la ISO 10218-1, se logra un entorno de capacitación de bajo costo, nulo riesgo físico y alta transferencia de conocimiento, alineándose con los estándares de la Industria 4.0."

## Objetivo Profesional:
Desarrollar  Simulación VR  en Industrias 4.0"  Especializándome en crear sistemas de control interactivos para robótica industrial en entornos de Realidad Virtual. Enfocado en la transición de controles manuales a sistemas inmersivos utilizando Unity y XR Interaction Toolkit.

## Fuentes Principales de Informacion:
- **Documentación de APIs:** XR Interaction Toolkit y la documentación de UnityEngine
- **Palbras Claves :** Digital Twin Unity,Industrial VR Training,Unity Robotics Hub,Inverse Kinematics VR,ROS-Unity-Integration

## Principios Ingenieria (Actualizaciones) :
Este simulador no es solo visual; se rige por principios de ingeniería real:
- **Seguridad Cinemática:** Límites de software para prevenir daños mecánicos y de personal.
- **Feedback HMI:** Confirmación visual y física del estado, según normas de usabilidad industrial.
- **Deadman Switch Logic:** El robot se detiene por defecto si el usuario pierde el control o la conexión.
  
## Herramientas Utilizadas (Actualizaciones) :
- **Desarrollo:** Unity 6000.3.6f1 ,Visual estudio Code
- **Lenguajes:** C#,PLC,Promps,
- **Framework:** XR Interaction Toolkit,
- **Optimizacion:** Herramientas de Inteligencia Artificial Generativa para refactorización de código y auditoría técnica.

## Aplicaciones Industriales (Actualizaciones) :
**Este proyecto se construye siguiendo directrices industriales internacionales para garantizar realismo y seguridad:**

ISO 13849-1 (Partes Relacionadas con la Seguridad de los Sistemas de Control): Implementación de la lógica de "Interruptor de Hombre Muerto". El movimiento se detiene inmediatamente ante la pérdida de señal (liberación del activador).

ISO 10218-1 (Robots para Entornos Industriales): Límites de software integrados (Clampado de Ejes) para evitar sobrepaso mecánico.

IEC 61131-3 (Controladores Programables): Uso de lógica de enclavamiento para prevenir comandos direccionales conflictivos.

Ergonomía UX/UI: Retroalimentación multimodal (Visual, Auditiva y Desplazamiento físico) para reducir la carga cognitiva del operador.

## 📖 Documentación Detallada (Notion)

Para un análisis más profundo sobre la metodología de investigación, bitácoras de desarrollo y gestión de activos, puedes consultar mis espacios de trabajo en Notion:

* [Bitácora de Desarrollo y Clases](LINK_A_NOTION) - Documentacion de cursos impartidos y Feedbacks
* [Especificaciones Técnicas y Diseño](LINK_A_NOTION) - Repositorio de Informacion
* [Gestión de Proyecto (Uso de VR)](LINK_A_NOTION) - Organización de tareas y recursos.

## Roadmap / Hoja de Ruta
- [x] **Phase 1: Foundations** - Basic Axis 2 movement and XR Input mapping.
- [x] **Phase 2: Industrial Safety** - Implementation of ISO 10218 limits and Interlock logic.
- [x] **Phase 3: Multimodal Feedback** - Physical button displacement and 3D Audio.
- [ ] **Phase 4: Full Kinematics** - Expansion to 3-axis and 6-axis control (In Progress).
- [ ] **Phase 5: AI Assistance** - Integration of AI-driven guidance for new operators.
- [ ] **Phase 6: Connectivity** - Digital Twin synchronization with real PLC (Future).

## Nivel: Básico (Realizado)
**Concepto:**  Interacción Directa.

Logro: Configuración de XR Interactables y mapeo de eventos (Select/Hover).

Dificultad: Baja.

Valor técnico: Demostrar entender el ciclo de vida de una interacción en VR (detección -> acción -> fin) en un Robot basico de 6 ejes al igual que intregar todos los conceptos basicos.

## Nivel: Intermedio (En Proceso ) 
**Concepto:**  Restricciones Cinemáticas y Seguridad en el proyecto donde  añadire Límites de Software.

Reto: No permitas que el robot gire infinitamente. Usa Mathf.Clamp o condicionales para que el robot se detenga a los -90° o 90°.

Dificultad: Media.

Por qué importa:  los robots Implementan "Soft Limits" para evitar roturas en sus propios cables. Implementacion enfocada en seguridad Industrial

## Nivel: Avanzado (En Proceso)
**Concepto:** HMI (Human-Machine Interface) Realista.

Reto 1: Movimiento Físico del Botón. No solo cambies el color; haz que el botón se desplace físicamente hacia adentro (eje local) cuando estaActivo sea true, y regrese al soltarlo.

Reto 2: Sentido Contrario. Crea un sistema de dos botones interconectados donde no puedan presionarse ambos a la vez (Lógica de enclavamiento).

Reto 3: Sonido Espacial. Añade un AudioSource al eje del robot con un sonido de motor eléctrico que aumente su tono (pitch) según la velocidad.

Dificultad: Alta.

Valor técnico: Principios en el dominio de la Experiencia de Usuario (UX) en VR.
