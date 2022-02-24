# 1. Styling Angular Applications

## 1.1. Links

Angular Style Guide
<https://angular.io/guide/styleguide>

## 1.2. Web Components

A Webcomponents are bundles of modular HTML, CSS and Javascript which are portions of whole app.

They are bundles to reuse.

### 1.2.1. Custom Elements

Create and use own elements.

### 1.2.2. HTML Templates

Fragments of markup. They are cloned to a referenced location.

### 1.2.3. Shadow DOM

## 1.3. Angular Component Structures

Angular Style Guide
<https://angular.io/guide/styleguide>

## 1.4. View Encapsulation

Angular supports 3 different Modes:
- None
- Emulated (default)
- ShadowDom

It can be changed by changing Component.encapsulation property.

### 1.4.1. Emulated

Should be used most of the time.

There are custom host and content attributes added to elements to get unique attributes for each component. This attributes are used to attach component style only to elements belongs to a component.

### 1.4.2. None

Can be used to use a global style and don't use component scope style.

### 1.4.3. ShadowDome

Is only supported in newer browser.

## 1.5. Component Style

Ways to add styles
- Embedded
  css is inside html template which is inside ts file
  Adds css into head.
- \<link\>
  css is in a seperate file but html is inside ts file
  Adds css into head.
- @import
  we can add imports to reference css file into our css file belonging to a component.
  Adds css into head.
- inline
  Add style directly into html elements. Not recomended as default
- styleUrls
  Is a property of component type to reference css files.
  Simple to setup.
  Adds css into head.

If using a external file you can use enhanced editor features like code completion or syntax highlighting to edit css code.

### 1.5.1. CSS Scoping Module

- :host
  Select the host of our component.
- :host-context
  looks in all parent nodes if a class name is there.
  Use it purposefully.
- ::ng-deep
  it's deprecated now

## 1.6. CSS Selectors

- element[attribute]
  Select all elements of type element containing a attribute with name attribute in it.
- :host 
- :host ul ::ng-deep a
  how elements needs to be nested to match

## 1.7. Scalable, Maintainable CSS/SCSS Architecture in Angular

everything is isolated 

no more bleed, conflict, or overriding

### clean, organized, structured, scalable

CSS Preprocessors should be used
### Topics 

- Global Styles
- Naming Conventions
- Relative Units & Predictability
- Selectors & Overrides
- Structure & Organization
- Mixins & Variables

#### Global Styles: 
