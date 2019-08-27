# The Route Object

A **route object** represents the state of the current active route. It contains parsed information of the current URL and the **route records** matched by the URL.

The route object is immutable. Every successful navigation will result in a fresh route object.

The route object can be found in multiple places:

* Inside components as this.$route

* Inside $route watcher callbacks

* As the return value of calling router.match(location)

* Inside navigation guards as the first two arguments:

```js
router.beforeEach((to, from, next) => {
    //`to` and `from` are both route objects
})
```

* Inside the scrollBehavior function as the first two arguments:

```js
const router = new VueRouter({
    scrollBehavior((to, from, savedPosition) {
        //`to` and `from` are both route objects
    })
})
```

