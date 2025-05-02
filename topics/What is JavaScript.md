# What is JavaScript?

JavaScript is a **dynamic**, **weakly typed** programming language primarily used to create **interactive**, **dynamic content** on webpages. It can be executed in web browsers or in other **host environments** like **Node.js**, enabling it to run not only on web pages but also on servers and various devices.

## 🕰️ History and Origins

JavaScript was created by **Brendan Eich** in **1995** while working at **Netscape**. It was initially called **LiveScript**, but later renamed to **JavaScript** to capitalize on Java's popularity at the time. Despite the name, **JavaScript** and **Java** are entirely different languages with distinct purposes.

JavaScript was standardized as **ECMAScript (ECMA-262)** by **ECMA International**. Major JavaScript engines include:

- **V8** (used in Google Chrome and Node.js)
- **SpiderMonkey** (used in Mozilla Firefox)
- **JavaScriptCore** (used in Apple Safari)

## ⚙️ Execution Model

Modern JavaScript is compiled **just-in-time (JIT)** at runtime by JavaScript engines. It combines features of both interpreted and compiled languages, allowing for fast execution and dynamic behavior.

## ✨ Key Characteristics

- **Dynamic Typing**: Variable types can change at runtime.
- **Weakly Typed**: Variables can implicitly convert between types.
- **Cross-Platform**: Runs in browsers, servers (Node.js), mobile apps, and more.
- **Event-Driven**: Ideal for handling events like clicks, input, and network responses.

---

## Why Study JavaScript?

JavaScript is one of the core technologies of the web, alongside **HTML** and **CSS**:

1. **HTML** – Structures the content.
2. **CSS** – Styles the content.
3. **JavaScript** – Adds interactivity and logic.

JavaScript allows developers to:

- Create interactive web apps.
- Modify content and styles dynamically.
- Handle events and validate forms.
- Communicate with servers (AJAX, Fetch API).
- Build full-stack apps using Node.js.

---

## JavaScript in Action

### 📝 Change HTML Content

```html
<p id="demo">Hello!</p>
<button onclick="changeText()">Click Me</button>

<script>
function changeText() {
  document.getElementById("demo").innerHTML = "You clicked the button!";
}
</script>
```

### 🖼️ Change HTML Attribute

```html
<img id="myImage" src="image1.jpg" width="200">
<button onclick="changeImage()">Change Image</button>

<script>
function changeImage() {
  document.getElementById("myImage").src = "image2.jpg";
}
</script>
```

### 🎨 Change CSS Styles

```html
<p id="text">Style me!</p>
<button onclick="changeStyle()">Change Style</button>

<script>
function changeStyle() {
  document.getElementById("text").style.color = "blue";
  document.getElementById("text").style.fontSize = "24px";
}
</script>
```

### 👻 Hide and Show Elements

```html
<p id="toggleText">Now you see me!</p>
<button onclick="hideText()">Hide</button>
<button onclick="showText()">Show</button>

<script>
function hideText() {
  document.getElementById("toggleText").style.display = "none";
}

function showText() {
  document.getElementById("toggleText").style.display = "block";
}
</script>
```

---

## 💡 Did You Know?

- **JavaScript ≠ Java**: Despite similar names, they have very different use cases.
- **Runs Everywhere**: JavaScript runs in the browser, on servers (Node.js), and even in desktop and mobile apps.
- **Standardized Language**: JavaScript follows the **ECMAScript** specification.
