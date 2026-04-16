# Enter-Modulo-3-Lab-11

---

## 🎯 Funcionalidad

* Centra el contenido en la pantalla usando Flexbox
* Muestra una tarjeta (`section`) con texto y título
* Incluye un botón circular posicionado de forma absoluta
* Se adapta a pantallas pequeñas con media queries

---

## 🧠 Cómo funciona

### 🔹 Centrado del layout

El `body` usa Flexbox para centrar la tarjeta:

```css
body{
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}
```

---

### 🔹 Estructura de la tarjeta

El `section` contiene todo el contenido:

* Usa `flex-direction: column` para organizar elementos en vertical
* Tiene `max-width` para limitar su tamaño
* `position: relative` permite posicionar el botón dentro

---

### 🔹 Botón flotante

El botón (`.boton`) está posicionado así:

```css
.boton {
  position: absolute;
  bottom: -2rem;
}
```

Esto hace que:

* El botón “salga” un poco de la tarjeta
* Se vea como un elemento flotante

---

### 🔹 Responsive (mobile)

Se usa un `@media` para ajustar el diseño en pantallas pequeñas:

* Reduce el tamaño del `section`
* Disminuye el tamaño del texto
* Ajusta el botón para que no se vea grande

```css
@media (max-width: 480px){
  section{
    width: 85%;
    max-width: 320px;
    padding: 1.5rem;
  }
}
```

---

## 🧱 Tecnologías usadas

* HTML
* CSS (Flexbox + Media Queries)
* Google Fonts (Manrope)

---

## ✅ Resultado

* Diseño centrado
* UI limpia
* Botón flotante moderno
* Adaptable a mobile

