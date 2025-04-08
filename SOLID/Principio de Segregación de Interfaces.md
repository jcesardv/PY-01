### 📘 Definición formal:

> **“Los clientes no deberían estar forzados a depender de interfaces que no usan.”**  
> — Robert C. Martin

---

### 💬 En palabras simples:

> **Mejor tener muchas interfaces pequeñas y específicas, que una sola grande y genérica.**

Cada clase debería implementar **solo los métodos que necesita**, no más.

---

## 🤕 ¿Qué pasa cuando se rompe ISP?

- Las clases terminan implementando métodos vacíos o inútiles.
    
- El sistema se vuelve **frágil**: cambios en una interfaz afectan a clases que no deberían verse afectadas.
    
- Cuesta más **probar, mantener o extender** el código.
    

---

## ❌ Ejemplo en Java que **viola ISP**:

![[Pasted image 20250408101652.png]]

### 🔴 Problema:

![[Pasted image 20250408101720.png]]


El `Robot` está obligado a implementar `eat()` porque la interfaz lo exige, aunque **no tiene sentido para él**.

---

## ✅ Refactor aplicando ISP

### 1️⃣ Dividimos en interfaces más pequeñas:

![[Pasted image 20250408101739.png]]

### 2️⃣ Las clases ahora implementan **solo lo que necesitan**:

![[Pasted image 20250408101755.png]]

---

## 🧠 Beneficios de ISP:

- Interfaces más limpias, más enfocadas.
    
- Código más flexible, más fácil de testear.
    
- Menos dependencias innecesarias.
    
- Se reduce el riesgo de introducir bugs al modificar interfaces grandes.
    

---

### 💡 Regla mental útil:

> "Si una interfaz empieza a crecer con métodos que **solo algunos clientes usan**, es momento de **dividirla**."