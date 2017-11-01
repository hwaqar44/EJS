"# EJS (https://github.com/hwaqar44/EJS)" 
A new Javascript UI Framework, Doing just for fun


 Simple default button

```
new E.button({
    text: "Click Me!",
    parent: E.getId('main') // appending button to a element of ID = 'main'
});
```

 Button colored green with white text color

```
new E.button({
    text: 'Black Button',
    color: 'green', // the text color is applied accordingly
    parent: E.getId('main') // appending button to a element of ID = 'main'

});
```
// Button with full width
```
new E.button({
    text: 'Full Width Btn',
    type: 'block',
    color: 'blue'
})
```
// Button with full width and align text to left
```
new E.button({
    text: 'Full Width Btn',
    type: 'block',
    color: 'blue',
    align: 'left' // or right
})
```

// Circular button
```
new E.button({
    text: '+',
    type: 'circle',
    color: 'yellow'
})
```
// Square button
```
new E.button({
    text: '+',
    type: 'button',
    color: 'yellow'
})
```
// button with custom style and disabled
```
new E.button({
    text: 'MY CUSTOM STYLED BUTTON',
    style: 'width: 250px; height:200px;',
    disabled: 'disabled'
})
```
// adding click event to button
```
new E.button({
    text: 'Click Me!',
    color: 'black',
    click: function(){
        alert(this.get('color'));
    }
})
```
//adding mouseover event
```
var i = 0;
new E.button({
    text: 'Mouse Over!',
    mouseover: function () {
        i++;
    },
    click: function(){
        alert(i+" times mouse over...");
    }
})
```
// button with icon with default settings
```
new E.button({
    text: 'HOME',
    icon: 'home',
})
```
// icon button with custom style
```
new E.button({
    icon: 'envelope',
    iconStyle: 'font-size: 36px;'
})
```
// icon align to right of button
```
new E.button({
    text: 'HOME',
    iconAlign: 'right',
    icon: 'home'
})
```
// icon align to the top of the text
```
new E.button({
    text: 'mail',
    iconAlign: 'top',
    icon: 'envelope',
    iconStyle: 'font-size: 26px;'
})
```
// Just icon as button
```
new E.button({
    icon: 'envelope',
    iconStyle: 'font-size: 20px;',
    click: function (event, element) { // event is mouse event, element is button element
        console.log(this.get('icon'));
    }
})
```
// custom image
```
new E.button({
    image: 'img/pdf.jpg',
    style: 'width: 100px; height: 40px;',
    iconStyle: 'width:70%; height: 70%;',
    color: 'white'
})
```
