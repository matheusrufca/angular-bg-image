# [![angular-translate](https://raw.github.com/angular-translate/angular-translate/canary/identity/logo/angular-translate-alternative/angular-translate_alternative_medium2.png)](http://angular-translate.github.io)

![Bower](https://img.shields.io/bower/v/angular-translate.svg) [![NPM](https://img.shields.io/npm/v/angular-translate.svg)](https://www.npmjs.com/package/angular-translate) [![cdnjs](https://img.shields.io/cdnjs/v/angular-translate.svg)](https://cdnjs.com/libraries/angular-translate) [![Build Status](https://img.shields.io/travis/angular-translate/angular-translate.svg)](https://travis-ci.org/angular-translate/angular-translate) ![License](https://img.shields.io/npm/l/angular-translate.svg) ![Code Climate](https://img.shields.io/codeclimate/github/angular-translate/angular-translate.svg) ![Code Coverage](https://img.shields.io/codeclimate/coverage/github/angular-translate/angular-translate.svg)

This is the repository for angular-bg-image.

bg-image is a directive to use CSS background-image attribute on elements.


## Install

### NPM
```
npm install --save-dev angular-bg-image
```

### Bower
```
bower install --save-dev angular-bg-image
```

### cdnjs
```
[CDNJS](https://cdnjs.cloudflare.com/ajax/libs/angular-moment/1.0.1/angular-moment.min.js)
* Download from github: [angular-moment.min.js](https://raw.github.com/urish/angular-moment/master/angular-moment.min.js)
```

## Getting started
-----
Include both **angular-bg-image.js** in your application.

```html
<script src="bower_components/angular-bg-image/dist/angular-bg-image.js"></script>
```

Add the module `mr` as a dependency to your app module:

```js
angular.module('app', ['mr']);
```

## Usage
-----

Use the directive like

```html
<div bg-image="model.pictureUrl" class="preview"></div>
```
or

```html
<div bg-image="{{getPictureUrl()}}" class="preview"></div>
```

```js
angular.module('app', ['mr'])
  .controller('DemoCtrl', function($scope){
    $scope.model {
      pictureUrl = 'http://i.imgur.com/xbiHEMe.jpg'
    };

    $scope.getPictureUrl = function(){
      return $scope.model.pictureUrl;
    };
  };
```

## License

Licensed under MIT.
