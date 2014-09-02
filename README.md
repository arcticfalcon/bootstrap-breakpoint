bootstrap-breakpoint
====================

Easy media queries mixin for Bootstrap 3

Usage:

Call the mixin with a list using **xs**, **sm**, **md** and **lg**.

Add **only** to break cascading upwards.

```
.my-class
{
  color: black;
  
  .break(sm only, {
  // min-width and max-width
    color: red;
  });

  .break(md, {
  // just min-width 
    color: blue;
  });

}

.my-other-class
{
  .break(sm only lg, {
  // not xs or md!
    color: white;
  });
}
```
