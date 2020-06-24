# Transitions That Will Wow Your Users
  <style>
  .fade
  {
          opacity:0.5;
  }
  .fade:hover
  {
          opacity:1;
  }

  </style>

 1. **Fade in** <br/>
Fade in effects are coded in two steps: first, you set the initial state; next, you set the change, for example on hover
```css
.fade
{
        opacity:0.5;
}
.fade:hover
{
        opacity:1;
}
```

2. **Change color** <br/>
Animating a change of color

```css
.color:hover
{
        background:#53a7ea;
}
```
3. **Grow & Shrink** <br/>
`To grow an element`, you used to have to use its width and height, or its padding. But now we can use CSS3’s transform to enlarge.
`Shrinking an element` is as simple as growing it. To enlarge an element we specify a value **greater than 1**, to shrink it, we specify a value **less than 1:**

```css
.grow:hover
{
        -webkit-transform: scale(1.3);
        -ms-transform: scale(1.3);
        transform: scale(1.3);
}
```
4. **Rotate elements**
CSS transforms have a number of different uses, and one of the best is transforming the `rotation of an element`. Give your div the **class “rotate”**
```css
.rotate:hover
{
        -webkit-transform: rotateZ(-30deg);
        -ms-transform: rotateZ(-30deg);
        transform: rotateZ(-30deg);
}
```
5. **Square to circle**
A really popular effect at the moment is transitioning a square element into a round one, and vice versa. With CSS, it’s a simple effect to achieve, we just transition the **border-radius property**.

```css
.circle:hover
{
        border-radius:50%;
}
```
6. **3D shadow** <br/>
3D shadows give a user feedback on their interactions and work with flat, or fake 3D interfaces.
```css
.threed:hover
{
        box-shadow:
                1px 1px #53a7ea,
                2px 2px #53a7ea,
                3px 3px #53a7ea;
        -webkit-transform: translateX(-3px);
        transform: translateX(-3px);
}
```
7. **Swing**
This animation simply moves the element left and right, now all we need to do is apply it:
```css
.swing:hover
{
        -webkit-animation: swing 1s ease;
        animation: swing 1s ease;
        -webkit-animation-iteration-count: 1;
        animation-iteration-count: 1;
}
```
8. **Inset border**
We can of course add a border to an element simply.
for ex to the class “border"
```css
.border:hover
{
        box-shadow: inset 0 0 0 25px #53a7ea;
}
```
