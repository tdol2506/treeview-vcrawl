Angular Treeview
================

Pure [AngularJS](http://www.angularjs.org) based tree menu directive.

[![ScreenShot](https://github.com/eu81273/angular.treeview/raw/master/img/preview.png)](http://jsfiddle.net/eu81273/8LWUc/17/)

## Installation

Copy the script and css into your project and add a script and link tag to your page.

```html
<script type="text/javascript" src="/angular.treeview.js"></script>
<link rel="stylesheet" type="text/css" href="css/angular.treeview.css">
```

Add a dependency to your application module.

```javascript
angular.module('myApp', ['angularTreeview']);
```

Add a tree to your application. See [Usage](#usage).

## Usage

Attributes of angular treeview are below.

- angular-treeview: the treeview directive
- tree-model : the tree model on $scope.
- node-id : each node's id
- node-label : each node's label
- node-children: each node's children

Here is a simple example.


```html
<div
    data-angular-treeview="true"
    data-tree-model="treedata"
    data-node-id="id"
    data-node-label="label"
    data-node-children="children" >
</div>
```

Example model:

```javascript
$scope.treedata = 
[
    { "label" : "User", "id" : "role1", "children" : [
        { "label" : "subUser1", "id" : "role11", "children" : [] },
        { "label" : "subUser2", "id" : "role12", "children" : [
            { "label" : "subUser2-1", "id" : "role121", "children" : [
                { "label" : "subUser2-1-1", "id" : "role1211", "children" : [] },
                { "label" : "subUser2-1-2", "id" : "role1212", "children" : [] }
            ]}
        ]}
    ]},
    { "label" : "Admin", "id" : "role2", "children" : [] },
    { "label" : "Guest", "id" : "role3", "children" : [] }
];     
```

## jsFiddle

[![ScreenShot](https://github.com/eu81273/angular.treeview/raw/master/img/jsfiddle.png)](http://jsfiddle.net/eu81273/8LWUc/17/)


## License

The MIT License.

Copyright ⓒ 2013 AHN JAE-HA.

See [LICENSE](https://github.com/eu81273/angular.treeview/blob/master/LICENSE)

