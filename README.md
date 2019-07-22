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
