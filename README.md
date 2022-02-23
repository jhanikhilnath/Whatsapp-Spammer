# Whatsapp-Spammer

My code Relies On two Classes from Whatsapp Web, which might change occasionally I will keep the repo updated if anything changes but it Might take Some time for me to update it,
If you find anything is not working feel free to open an issue

## The Code

```js
let message = prompt("Enter your message", "Hello"); // Can Replace prompt with a Set Text If You Like
let counter = parseInt(prompt("How many Times ?", 10)); // Can Replace prompt with a set number if you like
window.InputEvent = window.Event || window.InputEvent;
var event = new InputEvent("input", { bubbles: true });
var textbox = document.getElementsByClassName("_13NKt copyable-text selectable-text")[1];
// This is the main spam Bot
for (let index = 0; index < counter; index++) {
  textbox.innerHTML = message;
  textbox.dispatchEvent(event);
  document.getElementsByClassName("_4sWnG")[0].click();
}
```
