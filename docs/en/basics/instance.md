# Lvp Instance

The data verification function is absolutely single. So it is recommended to use a unique Lvp instance in your application. Lvp does not guarantee singletons using the singleton pattern like jQuery. Because there are multiple Lvpinstances at the same time, it will not affect the application.

```js
var lvp = new Lvp({ // configure });
```

When creating an Lvp instance, you can pass in a configuration object. You can also see a more complete list of configurations in [API Documentation] (/ api / config-object.md).

The prototype of this instance object has many built-in validation methods.

```js
// can be viewed via this API
Object.getPrototypeOf(lvp);
```

The methods you extend will be added to the Lvp instance itself.

All validation rule attribute names can be obtained on the ruleList attribute.

```js
lvp.ruleList;
```
