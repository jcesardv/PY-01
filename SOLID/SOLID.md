## ¿Qué es?

> **SOLID es una guía para escribir código limpio, flexible y a prueba del tiempo.**

Cuando lo aplicas bien:

- El código se adapta al cambio (como un buen lego).
    
- Es fácil de entender y modificar (no da miedo tocarlo).
    
- Permite crecer sin caos.

**SOLID** es un acrónimo que representa cinco principios de diseño orientado a objetos, propuestos por **Robert C. Martin** (Uncle Bob).  
Estos principios buscan hacer que el software sea:

---

### ✅ **Más mantenible**

> Es decir, que sea más fácil modificarlo o actualizarlo sin romper otras partes del sistema.  
> Por ejemplo, si haces un cambio en cómo se envían correos, no deberías afectar el cálculo de facturas.

---

### ✅ **Más extensible**

> Permite agregar nuevas funcionalidades sin tener que tocar el código que ya funciona.  
> Por ejemplo, puedes incluir un nuevo método de pago sin reescribir los existentes.

---

### ✅ **Más comprensible**

> El código es más claro, legible y organizado.  
> Cada clase tiene una función clara, lo que facilita que cualquier persona (incluyéndote en el futuro) lo entienda rápido.

---

### ✅ **Menos propenso a errores**

> Una buena estructura hace que sea menos probable introducir bugs al hacer cambios.  
> Las responsabilidades están bien separadas y los comportamientos bien definidos.


## 🧩 ¿Qué significan las siglas?

### 1. **S** - _Single Responsibility Principle_ (Principio de Responsabilidad Única)

> Una clase debe tener una sola razón para cambiar.

✅ **Beneficio:** Código más modular y fácil de mantener.

---

### 2. **O** - _Open/Closed Principle_ (Principio de Abierto/Cerrado)

> Las entidades (clases, módulos, funciones) deben estar **abiertas para extensión**, pero **cerradas para modificación**.

✅ **Beneficio:** Puedes agregar funcionalidades sin romper lo ya existente.

---

### 3. **L** - _Liskov Substitution Principle_ (Principio de Sustitución de Liskov)

> Las clases derivadas deben poder reemplazar a sus clases base **sin alterar el comportamiento esperado**.

✅ **Beneficio:** Promueve una jerarquía de clases más coherente y segura.

---

### 4. **I** - _Interface Segregation Principle_ (Principio de Segregación de Interfaces)

> Es mejor tener muchas interfaces específicas que una sola interfaz general.

✅ **Beneficio:** Los clientes solo dependen de lo que realmente usan.

---

### 5. **D** - _Dependency Inversion Principle_ (Principio de Inversión de Dependencias)

> Los módulos de alto nivel no deben depender de los de bajo nivel, **ambos deben depender de abstracciones**.

✅ **Beneficio:** Facilita el desacoplamiento, pruebas unitarias y cambios sin romper dependencias.

## 🎯 Beneficios Generales

- Mejor arquitectura de software
    
- Facilidad para hacer cambios sin romper todo
    
- Favorece las pruebas unitarias y TDD
    
- Código más legible, limpio y reutilizable
    
- Facilita el trabajo en equipo (menos dependencias cruzadas)