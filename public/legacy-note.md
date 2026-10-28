## 1. Native JavaScript Equivalents

1. `$(document).ready(callback)`
   - Native: `document.addEventListener("DOMContentLoaded", callback)`
2. `$("#name").val()`
   - Native: `document.querySelector("#name").value`
3. `.after(html)`
   - Native: `element.insertAdjacentHTML("afterend", html)`
4. `$(".error").remove()`
   - Native: `document.querySelectorAll(".error").forEach(el => el.remove())`
5. `.text(message).hide().fadeIn(400)`
   - Native: Set `textContent`, hide the element with CSS, then show it using the Web Animations API or a CSS transition.
6. `$form[0].reset()`
   - Native: `form.reset()`

## 2. Three Legacy Smells

1. Using `var` instead of modern `const` and `let`.
2. Using `$.trim()`, which is removed in jQuery 4; native JavaScript provides `String.prototype.trim()`.
3. Building HTML using strings and `.after()`, which can introduce security risks when untrusted data is inserted into HTML.
