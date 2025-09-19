**<> Price Icons**

The price icons are located in the symbols array at the top of the JavaScript file:

```javascript
const symbols = [
    {icon: '🧢'},
    {icon: '👕'},
    {icon: '🎟️'},
    {icon: '🍹'},
    {icon: '🎲'},
    {icon: '🚙'}
];
```
Each object in the array contains an icon that appears on the reels. You can modify these emojis with other ones or add new elements to the array.

**<> Result Messages**

The messages that appear after spinning the wheel are in the showResult function:
```javascript
function showResult(res) {
    const [a, b, c] = res;
    // ... code ...
    if (a === b && b === c) {
        let message = '';
        let prizeIcon = '';
        switch (a) {
            case '🚙': message = '¡Ganaste una camioneta SUV, felicidades!'; prizeIcon = '🚙'; break;
            case '🧢': message = '¡Felicidades, a estrenar gorra nueva!'; prizeIcon = '🧢'; break;
            case '👕': message = '¡Felicidades, tienes una playera nueva!'; prizeIcon = '👕'; break;
            case '🍹': message = '¡Ganaste una bebida gratis, salud!'; prizeIcon = '🍹'; break;
            case '🎟️': message = '¡15% de descuento en barra, a disfrutar!'; prizeIcon = '🎟️'; break;
            case '🎲': message = '¡Tiro gratis en una ruleta, todo al rojo!'; prizeIcon = '🎲'; break;
```

You can modify these prize messages by changing the text within each case.

**<> Font Settings**

The main font is configured in the CSS:
```css
body {
    font-family: 'Georgia', serif;
    /* ... other styles ... */
}
```
You can change 'Georgia' to any other available font or add custom fonts using @font-face.

**<> Text Styles**

Text styles for different elements are distributed throughout the CSS:
```css
    Main title: .page-title h1
    Subtitle: .page-title h2
    Symbols on reels: .symbol
    Result: .result
```
Each of these elements has its own font properties that you can customize according to your needs.
