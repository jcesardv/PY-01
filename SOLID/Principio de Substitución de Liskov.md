### 📘 Definición formal (por Barbara Liskov):

> _“Si S es un subtipo de T, entonces los objetos de tipo T pueden ser reemplazados por objetos de tipo S sin alterar las propiedades deseables del programa (exactitud, desempeño, etc.).”_

---

### 💬 En palabras simples:

> **Una subclase debe poder reemplazar a su clase base sin que el programa se rompa.**

Si creás una clase hija, **debe comportarse como una versión especializada de la clase padre**, **sin cambiar el contrato** (es decir, sin romper expectativas).

---

## 🤕 ¿Qué pasa cuando se viola LSP?

Cuando una subclase:

- Cambia el comportamiento esperado
    
- Lanza excepciones inesperadas
    
- Ignora partes del contrato (por ejemplo, no implementa todo)
    
- Hace cosas "raras" que el cliente no espera

## ❌ Ejemplo que viola LSP (en Java):

![[Pasted image 20250408101242.png]]
### 🧨 ¿Qué falla acá?

![[Pasted image 20250408101301.png]]
🔴 **El contrato de `Bird` dice que puede volar, pero Ostrich lo rompe**. No cumple LSP.

---

## ✅ Refactor aplicando LSP:

### 1️⃣ Creamos una jerarquía más precisa:

![[Pasted image 20250408101342.png]]
### 2️⃣ Ahora las subclases respetan su comportamiento esperado:

![[Pasted image 20250408101417.png]]

### 3️⃣ Uso correcto:

![[Pasted image 20250408101441.png]]

---

## 💡 Claves para aplicar LSP:

- Subclases deben **honrar el comportamiento** de sus padres.
    
- No lanzar errores donde no se esperan.
    
- No eliminar funcionalidades esperadas.
    
- Si una clase hija necesita "romper" el contrato de la base, ¡quizás **no** deba heredar de ella!