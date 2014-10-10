# Angular Odometer

angular-odometer lets you use [Hubspot Odometer](http://github.hubspot.com/odometer/) 
as angular directive

## Demo page

[Demo](http://bahaaldine.github.io/angular-odometer)

## Installation

Install depedencies using bower: 
```
bower install angular-odometer
```

Add js libraries to your application:
```html
	...
	<script src="bower_components/angular-odometer/dist/angular-odometer.js"></script>
    <script src="bower_components/odometer/odometer.min.js"></script>
    ...
```

Add css stylesheets to your application:
```html
    <link rel="stylesheet" href="bower_components/odometer/themes/odometer-theme-minimal.css"/>
```

Add ngOdometer module to you application
```javascript
	...
	angular
	  .module('myAwesomeApp', [
	    ...
	    'ngOdometer',
	    ...
	  ])
	...
```

## Usage

All you need is to place a ngOdometer with its attribute in your view like the following piece of code:
```javascript
	...
		<ng-odometer value="1234"></ng-odometer>
	...
```
`value`: the odometer value, can be dynamically set through controller scope variable, e.g. : `value="{{myScopeVariable}}"`. The value can also be refresh, the transition from one value to the other will be automatically done.

## Brower compatibility

Chrome: 35
Safari: 7