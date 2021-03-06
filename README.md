# SCSS+(A)BEM+Bootstrap4

## SCSS Pattern

### Classes

|Type|Class|
|---:|:---|
|Block:| `blockName`|
|Element:| `blockName__elementName`|
|Block + modifier:| `blockName -modifierName`|
|Element + modifier:| `blockName__elementName -modifierName`|

```html
<div class="blockName -modifierName">
	<div class="blockName__elementName -modifierName2"></div>
	<div class="blockName__elementName2"></div>
</div>
```

```scss
.blockName {
	/*...*/
	
	// Block modifiers
	& .-modifierName {
		/*...*/
	}
	
	// Elements
	&__elementName {
		/*...*/
		
		& .-modifierName2 {
			/*...*/
		}
	}
	
	&__elementName2 {
		/*...*/
	}
}
```

[Codepen example](https://codepen.io/_lacus/pen/gdqwxJ?editors=1100)


### TODO Highlight VSCode plugin settings to mark comments in SCSS files

Place this to .vscode/settings.json :

```json
"todohighlight.keywords": [
        "DEBUG:",
        "REVIEW:",
        {
            "text": "// Block modifiers",
            "color": "#000",
            "backgroundColor": "#4dabf7",
            "borderRadius": "4px",
            "border": "2px solid #74c0fc",
            "overviewRulerColor": "#74c0fc"
        },
        {
            "text": "// Elements",
            "color": "#000",
            "backgroundColor": "#3bc9db",
            "borderRadius": "4px",
            "border": "2px solid #66d9e8",
            "overviewRulerColor": "#66d9e8"
        },
	{
	    "text": "// Block variables",
            "color": "#000",
            "backgroundColor": "#38d9a9",
            "borderRadius": "4px",
            "border": "2px solid #63e6be",
            "overviewRulerColor": "#63e6be"
	}
],
```
## Basic SCSS file Structe 

```
sass/
|
|– component/
|   |– _buttons.scss
|   |– _carousel.scss 
|   |– _cover.scss 
|   |– _dropdown.scss
|   |– _navigation.scss
|   |– _grid.scss
|   |– _header.scss
|   |– _footer.scss
|   |– _sidebar.scss
|   |– _forms.scss
|   …  
|
|– pages/
|   |– _home.scss
|   |– _contact.scss
|   |– _blog.scss
|   |– _products.scss
|   …  
|
|– base/
|   |– _base.scss
|   |– _typo.scss
|   |– _reset.scss
|   …
|
|– vendors/
|   |– bootsrap/
|   |– bootsrap-extend/
|   |– fontawsome/
|   |– _jquery-ui.scss
|   …
|
|– _bootstrap-variables.scss	# To override bootstrap settings
|– _bootstrap-includes.scss	# To include Bootstrap modules separately
|– _variables.scss
|– _extends.scss
|– _mixins.scss
|– _functions.scss
|– app.scss  
```

## Atomic SCSS file Structe 


```
sass/
|
|– base/
|   |– _base.scss
|   |– _typo.scss
|   |– _reset.scss
|   …
|
|– vendors/
|   |– bootsrap/
|   |– bootsrap-extend/
|   |– fontawsome/
|   |– jquery-ui.scss
|   …
|
|– abstracts/
|   |– _bootstrap-variables.scss	# To override bootstrap settings
|   |– _bootstrap-includes.scss		# To include Bootstrap modules separately
|   |– _variables.scss
|   |– _extends.scss
|   |– _mixins.scss
|   |– _functions.scss
|   …
|
|– atoms/
|   |– _button.scss
|   |– _link.scss
|   |– _input.scss
|   |– _dropdown.scss
|   |– _image.scss
|   …  
|
|– molecules/
|   |– _cover.scss 
|   |– _grid.scss
|   |– _form.scss
|   |– _search.scss
|   …  
|
|– organisms/
|   |– _carousel.scss 
|   |– _navigation.scss
|   |– _header.scss
|   |– _footer.scss
|   |– _sidebar.scss
|   …  
|
|– templates/
|   |– _home.scss
|   |– _contact.scss
|   |– _blog.scss
|   |– _products.scss
|   …  
|
|– app.scss
|
```

## Resources

* http://getbem.com/
* https://css-tricks.com/abem-useful-adaptation-bem/
* http://atomicdesign.bradfrost.com/chapter-1/
* https://sass-guidelin.es/
* https://www.lullabot.com/articles/bem-atomic-design-a-css-architecture-worth-loving

* https://marketplace.visualstudio.com/items?itemName=wayou.vscode-todo-highlight

