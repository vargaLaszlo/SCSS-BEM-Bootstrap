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
