# Paper User Picture

[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/petja/paper-userpicture)

`paper-userpicture` lets you create user avatars. If user doesn't have picture set, we'll automatically create placeholder containing user name initials.

## Styling

Custom property | Description | Default
----------------|-------------|----------
`--paper-userpicture-size` | The size of picture | `5em`
`--paper-userpicture-text-size` | The font-size of the placeholder initials | `calc(var(--paper-userpicture-size) / 2)`

## Demos

### Basic example

You only need `user-id` and `user-name` attributes defined

<!---
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="paper-userpicture.html">
    <link rel="import" href="../paper-styles/paper-styles.html">
    <style>body{font-family:'Roboto'}.users{display:flex;}.users paper-userpicture{flex:1;}</style>
    <div class="users">
        <next-code-block></next-code-block>
    </div>
  </template>
</custom-element-demo>
```
-->
```html
<paper-userpicture user-id="AAA" user-name="Petja"></paper-userpicture>
<paper-userpicture user-id="BBB" user-name="Oliver"></paper-userpicture>
<paper-userpicture user-id="CCC" user-name="Luke"></paper-userpicture>
<paper-userpicture user-id="DDD" user-name="Yusef"></paper-userpicture>
```

### Show name under the picture

Add `show-name` attribute to show name of user under the picture

<!---
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="paper-userpicture.html">
    <link rel="import" href="../paper-styles/paper-styles.html">
    <style>body{font-family:'Roboto'}.users{display:flex;}.users paper-userpicture{flex:1;}</style>
    <div class="users">
        <next-code-block></next-code-block>
    </div>
  </template>
</custom-element-demo>
```
-->
```html
<paper-userpicture show-name user-id="EEE" user-name="Henry"></paper-userpicture>
<paper-userpicture show-name user-id="FFF" user-name="Thomas"></paper-userpicture>
<paper-userpicture show-name user-id="GGG" user-name="Michael"></paper-userpicture>
<paper-userpicture show-name user-id="HHH" user-name="Leo"></paper-userpicture>
```

### Use real user picture

And of course, if user has its picture set, you can show it by using `image` attribute as the reference to the URL.

<!---
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="paper-userpicture.html">
    <link rel="import" href="../paper-styles/paper-styles.html">
    <style>body{font-family:'Roboto'}.users{display:flex;}.users paper-userpicture{flex:1;}</style>
    <div class="users">
        <next-code-block></next-code-block>
    </div>
  </template>
</custom-element-demo>
```
-->
```html
<paper-userpicture image="http://lorempixel.com/160/160?1" user-id="III" user-name="Henry"></paper-userpicture>
<paper-userpicture image="http://lorempixel.com/160/160?2" user-id="JJJ" user-name="Thomas"></paper-userpicture>
<paper-userpicture image="http://lorempixel.com/160/160?3" user-id="KKK" user-name="Michael"></paper-userpicture>
<paper-userpicture image="http://lorempixel.com/160/160?4" user-id="LLL" user-name="Leo"></paper-userpicture>
```
