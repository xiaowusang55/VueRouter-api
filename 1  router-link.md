# `<router-link>`

`<router-link>` is the component for enabling user navigation in a router-enabled app.
The target location is specified with the `to` prop. It renders as an `<a>` tag with correct `href` by default, but can be configured with the `tag` prop. In addition, the link automatically gets an active CSS class when the target route is active.

`<router-link>` is preferred over hard-coded `<a href="...">` for the following reasons:

* It works the same way in both HTML5 history mode and hash mode, so if you ever decide to switch mode, or when the router falls back to hash mode in IE9, nothing needs to be changed.

* In HTML5 history mode, router-link will intercept the click event so that the browser doesn't try to reload the page.

* When you are using the base option in HTML5 history mode, you don't need to include it in to prop's URLs.


