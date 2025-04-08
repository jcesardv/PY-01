## 🟣 **D – Dependency Inversion Principle (DIP)**

### 📘 Definición formal:

> **“Los módulos de alto nivel no deberían depender de módulos de bajo nivel. Ambos deben depender de abstracciones. Las abstracciones no deben depender de los detalles, los detalles deben depender de las abstracciones.”**  
> — Robert C. Martin

---

### 💬 En palabras simples:

> **No hagas que las clases dependan directamente de otras clases concretas. Hacelas depender de interfaces o abstracciones.**

---

## 🔍 ¿Qué quiere decir esto?

- **Módulos de alto nivel** = reglas de negocio, lógica central
    
- **Módulos de bajo nivel** = detalles técnicos (bases de datos, APIs, archivos, etc.)
    

👉 El código central debería trabajar con **interfaces**, y no con **implementaciones específicas**.

---

## ❌ Ejemplo que **viola DIP** (Java):

![[Pasted image 20250408102022.png]]

### 🔴 Problemas:

- Si querés usar otro tipo de notificación (SMS, WhatsApp), **tenés que modificar** `Notification`.
    
- Está **acoplado** a `EmailService`.
    

---

## ✅ Refactor aplicando DIP:

### 1️⃣ Crear una **abstracción** (interfaz):

![[Pasted image 20250408102045.png]]

### 2️⃣ Implementaciones concretas:

![[Pasted image 20250408102108.png]]


### 3️⃣ Módulo de alto nivel depende de la abstracción:

![[Pasted image 20250408102125.png]]

### 4️⃣ Uso flexible:


![[Pasted image 20250408102141.png]]

---

## 🧠 Beneficios de aplicar DIP:

- 🔁 Cambiás implementaciones **sin tocar** el código central
    
- 🧪 Más fácil de testear (podés inyectar mocks)
    
- 📦 Código más modular y desacoplado
    
- 📈 Mucho más extensible
    

---

## 💡 Regla mental útil:

> **"Depende de lo que el código necesita hacer, no de cómo se hace."**  
> (Ej: Necesito _enviar un mensaje_, no saber _cómo se envía_.)