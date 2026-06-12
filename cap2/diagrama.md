# Diagrama de flujo 

**[Agrega un diagrama de flujo para tener una guía visual del proceso]**

**EJEMPLO:**

```{mermaid}
flowchart TD
    %% Nodos iniciales y Paso 1
    Start([Inicio del Proceso]) --> P1[Paso 1: Preparación y Prework]
    
    %% Paso 2
    P1 --> P2[Paso 2: Rompehielos y Validación]
    P2 --> Cond1{¿Objetivo claro y<br>priorizado?}
    Cond1 -- No --> Ayuda[Ayudar a priorizar el dolor principal]
    Ayuda --> P2
    Cond1 -- Sí --> P3
    
    %% Paso 3
    P3[Paso 3: Configuración Core] --> Cond2{¿Tiene la feature<br>configurada?}
    Cond2 -- No --> ConfNuevo[Configurar en vivo o definir deadline]
    Cond2 -- Sí --> Valida[Validar funcionamiento y optimizar]
    ConfNuevo --> P4
    Valida --> P4
    
    %% Paso 4
    P4[Paso 4: Identificación de Oportunidades] --> Cond3{¿Existe necesidad<br>adicional?}
    Cond3 -- Sí --> Pitch[Aplicar Pitch Natural / Upsell]
    Cond3 -- No --> P5
    Pitch --> P5
    
    %% Paso 5
    P5[Paso 5: Cierre y Siguientes Pasos] --> Asigna[Asignar Tareas y Pedir CSAT]
    Asigna --> Cond4{¿Requiere sesión<br>adicional?}
    Cond4 -- Sí --> Agenda[Agendar próxima sesión y enviar Kit]
    Cond4 -- No --> FinCierre[Enviar Kit y cerrar proceso]
    
    %% Fin
    Agenda --> Termino([Fin de la Sesión])
    FinCierre --> Termino
    
    %% Estilos
    classDef fase fill:#f9f9f9,stroke:#333,stroke-width:2px;
    class P1,P2,P3,P4,P5 fase;
```
