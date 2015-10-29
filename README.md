# ElementalJS

#### a DOM Manipulation library, simple and to the point

## Built by AppIns and CrazyGuy108

### Install:
```html
<head>
<!-- NOTE: We recommend Elemental.min.js for faster load times -->
<script src="Elemental.min.js"></script>
<script src="YourScriptFile.js"></script>
</head>
```

### Example:
```javascript
// Create NewDiv
var NewDiv = new Element("DIV");
  // Append NewDiv to body
  NewDiv.eAppendTo(document.body);
  // Identify NewDiv with an id
  NewDiv.eIdentify("NewDiv", undefined);
// NewP to store text
var NewP = new Element("P");
  // Append it to #NewDiv
  NewP.eAppendTo(eSel("#NewDiv"));
  // Set innerHTML to example
  NewP.eProperty("innerHTML", "Example");
```
will create a new div with the id NewDiv and append a p element to it, with the text "Example"


interacts well with HTML, jQuery, and CSS
```javascript
// Create a new div
var NewDiv = new Element("DIV");
  // Give the div an id
  NewDiv.eIdentify("NewDiv", "DivClass");

// JQuery can interact with this element
$("#NewDiv").hide();
```

```CSS
/* NOTE: Css can interact with the class */
.DivClass {
  text-align: center;
  font-size: 20px;
}
```

Create a new Element() from an existing one
```javascript
// Get the element with the id "textelement"
var i = new Element("#textelement");
  // Set the innerHTML (text between tags)
  i.eProperty("innerHTML", "I have changed everything!");
  // Change the style
  i.eStyle("backgroundColor", "#cbcbcb");
  // Return the id of the element and set it as x
  var x = i.eReturn("id");

// Get the element with the id "showcase"
var y = new Element("#showcase");
  // Append the old element to it
  y.eAddChild(eSel("#textelement"));
// Return the className of y and set it to id
var class = y.eReturn("className");
```

### Our library is small
Elemental.min.js takes up about 2.5 KB and without the manual it only takes up about 700 Bytes.
See ElementalNm.min.js. Much smaller than many other libraries.
###### This library may be updated and become larger.
