**Navegación:**  
[Inicio](index.md) | [Página 2](pagina2.md) | [Página 3](pagina3.md)

# Página 2 – Componentes del Modelo de Von Neumann

El modelo de **Von Neumann** se basa en un conjunto de componentes fundamentales que cooperan para ejecutar programas.

---

## Componentes esenciales

- **CPU (Unidad Central de Procesamiento)**
- **Memoria**
- **Entrada/Salida (I/O)**
- **Buses**

---

!!! info "Relación entre componentes"
    Todos los componentes del sistema comparten el **mismo bus**, lo que da lugar al conocido *cuello de Von Neumann*.

---

## Diagrama ilustrativo

![Von Neumann Diagram](img/componentes.png)

---

## Ejemplo de código (flujo simplificado)

```python
pc = 0
instruction = memory[pc]
execute(instruction)
pc += 1