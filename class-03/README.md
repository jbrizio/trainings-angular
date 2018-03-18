# Class 03 - Angular Components

The third class was given the 13/03/18 via Webex.
On this, the teacher introduces to us and start talking about the following topics mentioned below.

## Index
- Structure
- Naming
- Features
- Life Cycle
- Component Interaction
- Bootstrap
- SASS

## Structure
The architecture of Angular is based on inherit between components.

Good practices mentioned:
- Put the application code on the `src` folder
- One module for each feature of our application
- You can put commonly used directives, pipes, and components into one module and then import just that module wherever you need it in other parts of your app

## Naming
Names of components should be consistent and descriptive.

Is recommendable to use the following convention when creates a file:

`feature.type.ts`

- Where the feature is the descriptive name

- Where type can be:
    - `.service`
    - `.component`
    - `.pipe`
    - `.module`
    - `.directive`

The name of classes and files should be the same:

- `export class UsersComponent { } =>  users.component.ts`
- `export class AgeValidationDirective{ } => age-validation.directive.ts`

## Features
Component decorator allows you to mark a class as an Angular component and provide additional metadata that determines how the component should be processed, instantiated and used at runtime.

Metadata Properties

- `animations` - list of animations of this component
- `changeDetection` - change detection strategy used by this component
- `encapsulation` - style encapsulation strategy used by this component
- `entryComponents` - list of components that are dynamically inserted into the view of this component
- `exportAs` - name under which the component instance is exported in a template
- `host` - the map of the class property to host element bindings for events, properties and attributes
- `inputs` - list of class property names to data-bind as component inputs
- `interpolation` - custom interpolation markers used in this component's template
- `moduleId` - ES/CommonJS module id of the file in which this component is defined
- `outputs` - list of class property names that expose output events that others can subscribe to
- `providers` - list of providers available to this component and its children
- `queries` - configure queries that can be injected into the component
- `selector` - CSS selector that identifies this component in a template
- `styleUrls` - list of URLs to stylesheets to be applied to this component's view
- `styles` - inline-defined styles to be applied to this component's view
- `template` - inline-defined template for the view
- `templateUrl` - URL to an external file containing a template for the view
- `viewProviders` - list of providers available to this component and its view children

## Life Cycle
A component has a lifecycle managed by Angular.

Angular creates it, renders it, creates and renders its children, checks it when its data-bound properties change, and destroys it before removing it from the DOM. Angular offers lifecycle hooks that provide visibility into these key life moments and the ability to act when they occur:

- `ngOnChanges()`
- `ngOnInit()`
- `ngDoCheck()`
- `ngAfterContentInit()`
- `ngAfterContentChecked()`
- `ngAfterViewInit()`
- `ngAfterViewChecked()`
- `ngOnDestroy()`

## [Component Interaction](https://angular.io/guide/component-interaction)
On this section was explained how are the different scenarios in which two or more components share information:

- Passing the reference of one component to another
- Communication through parent component
- Communication through Service

## [Bootstrap](https://getbootstrap.com)
Bootstrap is a free front-end framework for faster and easier web development. Bootstrap includes HTML and CSS based design templates for typography, forms, buttons, tables, navigation, modals, image carousels and many other, as well as optional JavaScript plugins.

Installing this how to dependency with npm:

`npm install bootstrap --save`

After of that, you need to import with the following line in your stylesheet file:

`@import "~bootstrap/dist/css/bootstrap.css"`

## [SASS](https://sass-lang.com)
Sass (Syntactically Awesome Style Sheets) is an extension of CSS that enables you to use things like variables, nested rules, inline imports and more. It also helps to keep things organized and allows you to create style sheets faster.

Some qualities that introduce SASS:
- Variables
- Nesting
- Partials
- Import
- Mixins
- Extend
- Operators
