﻿# ng2-pickadate

An Angular2 component for pickadate.js. 
See the [changelog](./CHANGELOG.md) for more information.


### Demo
* Demo can be found at [https://cschroeter.github.io/ng2-pickadate/](https://cschroeter.github.io/ng2-pickadate/) 


### Usage

 ```typescript
import { Component } from '@angular/core';
import { Ng2Pickadate } from 'ng2-pickadate/ng2-pickadate';
 
 @Component({
   selector: 'my-app',
   template: `<ng2-pickadate [min]="minDate" (select)="onSelect($event)"></ng2-pickadate>`,
   directives: [Ng2Pickadate]
 })
 export class MyAppComponent {
     public minDate: Date = new Date();
     
     public onSelect(timestamp): void {
         console.log(timestamp)
     }
 }
 
 ```


### Requirements

* [Angular2](https://angular.io/)
* [pickadate](http://amsul.ca/pickadate.js/)
* [JQuery](http://jquery.com/)


### Installation

* [Angular CLI Configuration (SystemJS)](./docs/angular-cli.md)


### Themes

Themes will be supported later on. For the moment you can use the default css styles provided by pickadate.js

```html
<link href="https://cdnjs.cloudflare.com/ajax/libs/pickadate.js/3.5.6/compressed/themes/default.css" rel="stylesheet">
<link href="https://cdnjs.cloudflare.com/ajax/libs/pickadate.js/3.5.6/compressed/themes/default.date.css" rel="stylesheet">
```