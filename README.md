# gedit-snippets-angular

AngularJS snippets for GEdit

## How to use

In GEdit, open **Tools** > **Manage snippets...** and click the **Import snippets** button below the snippets list. Navigate
to the folder where you cloned this repository and select the **js.xml** file. That's it! The snippets are now imported
and available in any Javascript file.

To use the snippets, just type the snippet name and hit tab.

## Snippets list

### ngfor

Generates an angular.forEach statement:
```Javascript
angular.forEach(${1:collection}, function (value, key) {
	$0
});
```

### nglog

Generates a $log.info call:
```Javascript
$log.info('${1:message}');
```

### nglogwarn

Generates a $log.warn call:
```Javascript
$log.warn('${1:message}');
```

### nglogerr

Generates a $log.error call:
```Javascript
$log.error('${1:message}');
```

### ngb

Generates a $scope.$broadcast call:
```Javascript
$scope.$broadcast('${1:eventName}', ${2:args});
```

### nge

Generates a $scope.$emit call:
```Javascript
$scope.$emit('${1:eventName}', ${2:args});
```

### ngf

Adds a function to the $scope object:
```Javascript
$scope.${1:functionName} = function (${2:args}) {
	$0
};
```

### ngv

Adds a variable to the $scope object:
```Javascript
$scope.${1:varName} = ${2:value};
```

### ngon

Adds an event listener to the $scope object:
```Javascript
$scope.$on('${1:eventName}', function (event, args) {
	$0
});
```

### ngw

Adds a $watch statement on the $scope object:
```Javascript
$scope.$watch('${1:expression}', function (newValue, oldValue) {
	$0
});
```
