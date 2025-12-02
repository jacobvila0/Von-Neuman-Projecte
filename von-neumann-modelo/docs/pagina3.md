# Página 3 – Comparación con Harvard

La arquitectura **Harvard** y la de **Von Neumann** se diferencian principalmente en cómo gestionan la memoria y los buses del sistema.

---

## Diferencias principales

| Característica | Von Neumann | Harvard |
|----------------|-------------|---------|
| Memoria        | Única para datos e instrucciones | Separada |
| Buses          | Bus único compartido | Buses independientes |
| Velocidad      | Limitada por el cuello de Von Neumann | Mayor paralelismo |
| Flexibilidad   | Simpler | Más compleja pero eficiente |

---

!!! warning "Punto clave"
    En Harvard la CPU puede **leer datos y leer instrucciones al mismo tiempo**, lo cual **no es posible** en el modelo de Von Neumann.

---

## Imágenes de referencia

**Arquitectura Von Neumann**  
![VN](https://upload.wikimedia.org/wikipedia/commons/8/8b/Von_Neumann_Architecture.svg)

**Arquitectura Harvard**  
![Harvard](https://upload.wikimedia.org/wikipedia/commons/6/6f/Harvard_architecture.svg)

---

## Código ilustrativo

```pseudo
# Von Neumann (memoria única)
MEM[100] = 8
instruction = MEM[20]

# Harvard (memoria separada)
DATA_MEM[100] = 8
INSTR_MEM[20] = LOAD
