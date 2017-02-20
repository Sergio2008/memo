# Angular

## How to angular

### 1. we created a new module /Creation d'un nouveau module
```
var app = angular.module("myApp", []);
```

### 2. called a directive / appellons une directive
```
<body ng-app="myApp">

```

### 3. created a new controller /creation d'un controller
```
app.controller('MainController', ['$scope', function($scope) { 
  $scope.title = 'Top Sellers in Books'; 
}]);
```

### 4. create a directive that defines the controller scope /creation d'un controller qui défini le controlleur de scope
```
<div class="main" ng-controller="MainController">
```

###  5. we accessed $scope.title using {{ title }} /acceder aux données
```
{{ title }}
```

###  6. formater /filtrer les données
```
{{ title | filtre }}
```
