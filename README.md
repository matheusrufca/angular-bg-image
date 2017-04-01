angular-bg-image
==============

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

### CDN
```hmtl
<script src="https://cdn.rawgit.com/matheusrufca/angular-bg-image/master/dist/angular-bg-image.js"></script>
```

## Getting started

Include both **angular-bg-image.js** in your application.

```html
<script src="bower_components/angular-bg-image/dist/angular-bg-image.js"></script>
```

Add the module `mr` as a dependency to your app module:

```js
angular.module('app', ['mr']);
```


## Usage

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
