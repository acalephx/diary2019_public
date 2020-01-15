# ng-keydown

https://stackoverflow.com/questions/19583496/can-angularjs-ng-keyup-pass-in-which-key-was-pressed

```html
<div ng-model="data" 
     onchange = "angular.element(this).scope().myFunction(this.name)"
     ng-keydown="listenK($event)">
```

```js
$scope.listenK = function (e) {
  console.log("listenK",e);
  if (e.keyCode==13) {
      console.log("press Enter");
  }
};
```

 
# onChange

https://www.jianshu.com/p/ee59741463da

```html
<div ng-model="data" 
     onchange = "angular.element(this).scope().myFunction(this.name)">
```

https://stackoverflow.com/questions/38378972/difference-between-on-change-and-ng-change

https://www.w3schools.com/angular/angular_events.asp

