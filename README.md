# TicketTimeTrackingAngularPolarisApp

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 1.3.0.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `-prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).
Before running the tests make sure you are serving the app via `ng serve`.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).

## Custom calendar component documentation 

### component is added to the shared library you dont need to add/import this module 

Below is the snapshot of the component 

```HTML
<polaris-date-picker 
 type="both" 
[(ngModel)]="date"
[minDate]= "minDate" 
[maxDate]="maxDate" 
mode="range" 
zone="America/New_York" 
(change)="testCall($event)">
</polaris-date-picker>
```
Below attribute is for the picker type 
```JavaScript
 type="both" | "time" | "calender"

 Default : "calender"
```
Below attribute is to set start date for the calender
```JavaScript
[minDate]= "minDate" 
Defualt : null
```
Below attribute is to set maximum allowed date for the calender
```JavaScript
[maxDate]="maxDate" 
Defualt : null
```
Below attribute is to set mode for the  calender 
```JavaScript
mode="range" || 'single' || 'multiple'
Default : 'single'
```
Below attribute is to set timezone for the  calender 
```JavaScript
zone="America/New_York" 
```
Below attribute is to catch the change emitter for the calender

```JavaScript
(change)="testCall($event)"
```

