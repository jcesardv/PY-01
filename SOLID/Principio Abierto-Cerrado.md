### 📘 Definición clara:

> **“Las entidades de software (clases, módulos, funciones) deben estar abiertas para su extensión, pero cerradas para su modificación.”**  
> — Bertrand Meyer

### 🔍 ¿Qué significa?

Significa que **puedes extender el comportamiento de una clase sin tener que modificar su código fuente**.

✅ Esto se logra comúnmente usando:

- **Herencia** (polimorfismo)
    
- **Interfaces**
    
- **Abstracciones (estrategias, factory, etc.)**
    

---

## 🤯 ¿Por qué es útil?

Porque **modificar código viejo puede romper cosas que ya funcionaban**.  
En cambio, si extiendes el sistema agregando nuevas clases, puedes mejorar o adaptar sin poner en riesgo lo existente.

---

## 🚨 Casos donde se rompe este principio:

### ❌ Ejemplo en Java que **viola OCP**:

![[Pasted image 20250408100624.png]]

🔴 **Problema:**  
Cada vez que agregas un nuevo tipo de pago, debes **modificar** la clase. Esto viola OCP.

---

## ✅ Refactor usando OCP: abierto a extensión, cerrado a modificación

### 1️⃣ Crear una interfaz:

![[Pasted image 20250408100645.png]]

### 2️⃣ Implementaciones específicas:

![[Pasted image 20250408100725.png]]

### 3️⃣ Ahora, el procesador ya no necesita saber los tipos:

![[Pasted image 20250408100749.png]]

### 4️⃣ Uso:

![[Pasted image 20250408100807.png]]

---

## 🧠 Ventajas después de aplicar OCP:

- Para agregar un nuevo método de pago, **solo creas una nueva clase**, sin tocar las demás.
    
- Reducís el riesgo de romper código existente.
    
- Tu sistema escala mejor (abierto a crecimiento).