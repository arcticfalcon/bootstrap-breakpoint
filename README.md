bootstrap-breakpoint
====================

Easy media queries mixin for Bootstrap 3

Usage:
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
```
