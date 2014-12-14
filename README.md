# angular-bind-compile
An angular plugin provides bind html with compilation.

## Download
[Compress](https://raw.github.com/emn178/angular-bind-compile/master/build/angular-bind-compile.min.js)  
[Uncompress](https://raw.github.com/emn178/angular-bind-compile/master/src/angular-bind-compile.js)

## Demo
[ngBindCompile](http://emn178.github.io/angular-bind-compile/samples/ng-bind-compile/)  

## Usage
Add the ngBindCompile module as a dependency to your application module:
```JavaScript
var myAppModule = angular.module('MyApp', ['ngBindCompile'])
```

## ngBindCompile
The ngBindCompile directive allows you to bind html with compilation. See also [ngBindHtml](https://docs.angularjs.org/api/ng/directive/ngBindHtml).

### Directive Info
This directive executes at priority level 0.

### Usage
as attribue:
```HTML
<ANY
  ng-bind-compile="">
...
</ANY>
```
### Arguments
| Param | Type | Details |
|:-----|:-------|-------|
|ngBindCompile   |expression     |Expression to evaluate.    |

### Example
HTML:
```HTML
<div ng-bind-compile="html"></div>
```
JavaScript:
```JavaScript
$scope.html = $sce.trustAsHtml('<button ng-click="click()">Click</button>');
```
## License
The project is released under the [MIT license](http://www.opensource.org/licenses/MIT).

## Contact
The project's website is located at https://github.com/emn178/angular-bind-compile  
Author: emn178@gmail.com
