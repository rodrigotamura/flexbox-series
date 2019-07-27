# Description
Flexbox series. Each commit will contain new feature. It is a self training of flexbox usage.

## 01 - Introduction
For practicing with flexbox, first, we need a CONTEINER. Within this container we put some ITEMS.
In the CSS of CONTAINER class we will add `display:flex` to initialize the usage of FlexBox.
```
.container {
  display: flex;
  height: 100vh;
}
```
The `height: 100vh` will stretch the height of container 100% according to the viewport (90vh means 90% of viewport height).

## 02 - Direction
We can set the direction of the container's items by `flex-direction` property. The values may be `row`, `row-reverse`, `column` or `column-reverse`. The default value is `row`.
```
.container {
  display: flex;
  height: 100vh;
  flex-direction: column;
}
```

## 03 - Wrapping elements with flexbox
By default, flex items will all try to fit onto one line. Wrap property will put them wrapped onto multiple lines, from top to bottom.
<pre>
.container {
    display: flex; /* it is making its children as flex items */
    border: 10px solid goldenrod;
    height: 100vh; /* Viewport Height - it will automatically adjust (strech) the height of the element */
    <b>flex-wrap: wrap;</b>
}
</pre>

## 04 - Setting order on items
We can set the order of a group of items in a flex container with `order` property.
By default each item of flex container `order` is 0 - zero.
<pre>
.container{
  display: flex;
}
.container .item01 {
  <b>order: 1;</b>
}
.container .item02 {
  <b>order: 2; /* come after .item01 */</b>
}
</pre>
