## SRP – Single Responsibility Principle (Principio de Responsabilidad Única)

### 📘 Definición:

> **Una clase (o módulo) debe tener una única razón para cambiar**, lo que significa que debe estar enfocada en una única tarea o responsabilidad dentro del sistema.  
> Aplicar SRP hace que el software sea **modular, fácil de entender, probar, mantener y extender**.

Cuando una clase se encarga de múltiples cosas (como acceder a datos, procesar lógica, y manejar la interfaz), está **acoplada a demasiados contextos**, lo que aumenta el riesgo de errores cuando hay cambios.

## ❌ **ANTES – Violación de SRP (una clase hace demasiado)**

![[Pasted image 20250408095601.png]]

🔴 **Problemas:**

- `Invoice` calcula totales (negocio), guarda en base de datos (persistencia) **y** maneja impresión (presentación).
    
- Tiene múltiples razones para cambiar.
    

---

## ✅ **DESPUÉS – Aplicando SRP correctamente**

### 📦 `Invoice.java`

![[Pasted image 20250408095647.png]]
### 💾 `InvoiceRepository.java`

![[Pasted image 20250408095734.png]]

### 🖨️ `InvoicePrinter.java`

![[Pasted image 20250408095813.png]]

### 📦 `Item.java`

![[Pasted image 20250408095840.png]]
---

### 🧪 Ejemplo de uso:

![[Pasted image 20250408095907.png]]
---

## 🚀 Beneficios logrados:

- Cada clase tiene **una única responsabilidad**.
    
- Puedes cambiar la base de datos, el formato de impresión o la lógica de negocio **de forma independiente**.
    
- Mucho más fácil de probar, mantener y extender.