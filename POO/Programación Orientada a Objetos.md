> La **Programación Orientada a Objetos (POO)** es un paradigma de programación que organiza el software en **objetos**, los cuales combinan **datos (atributos)** y **comportamientos (métodos)**.

En lugar de escribir funciones sueltas, **modelás entidades del mundo real** (como un auto, un usuario o una factura) usando clases y objetos.

## 🧩 ¿Cuáles son los **pilares** de la POO?

1. ### **Abstracción**
    
    👉 Enfocarse en lo esencial, ocultando los detalles internos.  
    📌 Ejemplo: al usar un coche, no necesitás saber cómo funciona el motor, solo cómo conducirlo.
    
2. ### **Encapsulamiento**
    
    👉 Proteger los datos internos de un objeto, permitiendo el acceso controlado.  
    📌 Ejemplo: los atributos de una clase están privados y se acceden mediante getters/setters.
    
3. ### **Herencia**
    
    👉 Permitir que una clase **herede** atributos y métodos de otra.  
    📌 Ejemplo: `Perro` hereda de `Animal`.
    
4. ### **Polimorfismo**
    
    👉 Permitir que diferentes clases respondan al mismo método de forma distinta.  
    📌 Ejemplo: `Círculo` y `Rectángulo` tienen un método `dibujar()`, pero cada uno lo implementa a su manera.
    

---

## 🧱 ¿Cómo se usa POO en la práctica?

Cuando programás con POO, creás:

- **Clases** → plantillas para crear objetos
    
- **Objetos** → instancias de esas clases
    
- **Métodos** → comportamientos (funciones dentro de clases)
    
- **Atributos** → datos de cada objeto

## ✅ Beneficios de la POO:

- Código más **modular**, fácil de entender y mantener
    
- Reutilización gracias a **herencia**
    
- Facilita el crecimiento del sistema
    
- Ideal para modelar sistemas complejos y reales

## 🧱 **Primero, recordemos los 4 pilares de la POO:**

| Pilar               | ¿Qué representa?                                                              |
| ------------------- | ----------------------------------------------------------------------------- |
| **Abstracción**     | Ocultar detalles complejos, mostrar solo lo esencial.                         |
| **Encapsulamiento** | Proteger el estado interno del objeto; controlar el acceso a los datos.       |
| **Herencia**        | Reutilizar código mediante jerarquías de clases.                              |
| **Polimorfismo**    | Tratar objetos de diferentes clases de forma uniforme a través de interfaces. |

## 🔗 **Relación de cada principio SOLID con POO:**

|Principio SOLID|Relación con POO|Cómo se conecta|
|---|---|---|
|**S** – SRP (Single Responsibility)|✅ Encapsulamiento  <br>✅ Abstracción|Cada clase encapsula **una sola razón para cambiar** y **un propósito claro**, manteniendo su responsabilidad aislada.|
|**O** – OCP (Open/Closed)|✅ Polimorfismo  <br>✅ Abstracción|Utiliza **interfaces y herencia** para **extender** funcionalidades sin **modificar** código existente.|
|**L** – LSP (Liskov Substitution)|✅ Herencia  <br>✅ Polimorfismo|Garantiza que las **subclases sean sustitutos válidos** de las superclases, respetando los contratos.|
|**I** – ISP (Interface Segregation)|✅ Abstracción  <br>✅ Encapsulamiento|Promueve interfaces pequeñas y específicas, lo que **refuerza la separación de responsabilidades** y mejora la abstracción.|
|**D** – DIP (Dependency Inversion)|✅ Abstracción  <br>✅ Polimorfismo|Invierte las dependencias a favor de **interfaces**, permitiendo una arquitectura desacoplada y flexible.|
## 🎯 En resumen:

> La **POO provee las herramientas** (clases, objetos, herencia, interfaces),  
> y **SOLID guía cómo usarlas bien** para lograr un **diseño limpio, mantenible y escalable**.