# SCSS BEM Bootstrap

## File Structe

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
|– _variables.scss
|– _extends.scss
|– _mixins.scss
|– _functions.scss
|– app.scss  
```

## SCSS Pattern

```
.block {
	/*...*/
	
	// Block modifiers
	& .-modifier {
		/*...*/
	}
	
	// Elements
	&__element {
		/*...*/
		
		& .-modifier2 {
			/*...*/
		}
	}
	
	&__element2 {
		/*...*/
	}
}

```
### TODO Highlight settings to mark comments in SCSS files

Place this to .vscode/settings.json :

```
"todohighlight.keywords": [
	"DEBUG:",
	"REVIEW:",
	{
	    "text": "// Block modifiers",
	    "color": "#000",
	    "backgroundColor": "#4dabf7",
	    "borderRadius": "4px",
	    "border": "2px solid #74c0fc",
	},
	{
	    "text": "// Elements",
	    "color": "#000",
	    "backgroundColor": "#3bc9db",
	    "borderRadius": "4px",
	    "border": "2px solid #66d9e8",
	}
],
```

## Resources

http://atomicdesign.bradfrost.com/chapter-1/
https://sass-guidelin.es/

