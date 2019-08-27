# `<rotuer-view>`

The `<router-view>` component is a functional component that renders the matched component for the given path. Components rendered in `<router-view`> can also contain its own `<router-view>`, which will render components for nested paths.

Any non-name props will be passed along to the rendered component, however most of the time the per-route data is contained in the route's params.

Since it's just a component, it works with `<transition>` and `<keep-alive>`. When using the both together, make sure to use `<keep-alive>` inside:

```html
<transition>
    <keep-alive>
        <router-view></router-view>
    </keep-alive>
</transition>
```
