# Styling Angular Applications

## Links

Angular Style Guide
<https://angular.io/guide/styleguide>

## Web Components

A Webcomponents are bundles of modular HTML, CSS and Javascript which are portions of whole app.

They are bundles to reuse.

### Custom Elements

Create and use own elements.

### HTML Templates

Fragments of markup. They are cloned to a referenced location.

### Shadow DOM

## Angular Component Structures

Angular Style Guide
<https://angular.io/guide/styleguide>

## View Encapsulation

Angular supports 3 different Modes:
-None
-Emulated (default)
-ShadowDom

It can be changed by changing Component.encapsulation property.
### Emulated

Should be used most of the time.

There are custom host and content attributes added to elements to get unique attributes for each component. This attributes are used to attach component style only to elements belongs to a component.

### None

Can be used to use a global style and don't use component scope style.

### ShadowDome

Is only supported in newer browser.

## Component Style

Ways to add styles
-Embedded
  css is inside html template which is inside ts file
  Adds css into head.
-\<link\>
  css is in a seperate file but html is inside ts file
  Adds css into head.
-@import
  we can add imports to reference css file into our css file belonging to a component.
  Adds css into head.
-inline
  Add style directly into html elements. Not recomended as default
-styleUrls
  Is a property of component type to reference css files.
  Simple to setup.
  Adds css into head.

If using a external file you can use enhanced editor features like code completion or syntax highlighting to edit css code.



## CSS Selectors

Select all elements of type element containing a attribute with name attribute in it.
element[attribute]
