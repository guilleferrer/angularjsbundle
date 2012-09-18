angularjsbundle
===============

The angularjs bundle provides a basic template for an angular project and loads the assets requried by the www.angularjs.org project

Make your template to {% extends 'UdfAngularJSBundle::angular_base.html.twig' %}

For your project and you'll have a bootstraped version with the main assets for your Angular project

To configure just add :
```
// AppKernel.php
new Udf\AngularJSBundle\UdfAngularJSBundle()
````

```
// Edit your composer.json and add this line in the "require" object
"guilleferrer/angularjsbundle" :"dev-master"
```

This bundle FORCES you to have a MainCtrl function in javascript, that belongs to the the <body> tag :
````
<body ng-controller="MainCtrl"> 
...
</body>
```