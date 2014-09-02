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
    color: red;
  });

  .break(md, {
    color: blue;
  });

}

.my-other-class
{
  .break(sm only lg, {
    color: white;
  });
}
```

outputs:

```
.my-class {
  color: black;
}
@media (min-width: 768px) and (max-width: 991px) {
  .my-class {
    color: red;
  }
}
@media (min-width: 992px) {
  .my-class {
    color: blue;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .my-other-class {
    color: white;
  }
}
@media (min-width: 1200px) {
  .my-other-class {
    color: white;
  }
}
```
