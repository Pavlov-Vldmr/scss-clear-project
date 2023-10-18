# SCSS custom clear project


## Sass start

`sass --watch scss/index.scss:styles/index.css`

>[!IMPORTANT]
>**box-sizing: border-box** model used

## Containers

### Custom padding

To change padding edit `--getter-x` in `commoon.scss`
```bash
.
├───...
├───scss
│   ├───common    # common.scss
│   └───...    
└───...
```

### Container sizes
```
@media (min-width: 320px) {
  .container {
    width: auto;
    max-width: none;
  }
}

@media (min-width: 425px) {
  .container {
    max-width: 420px;
  }
}
@media (min-width: 768px) {
  .container {
    max-width: 720px;
  }
}
@media (min-width: 992px) {
  .container {
    max-width: 960px;
  }
}
@media (min-width: 1200px) {
  .container {
    max-width: 1140px;
  }
}
@media (min-width: 1400px) {
  .container {
    max-width: 1320px;
  }
}

```




## Media breacpoints 

### Structure
@media breackpoints *mixin* uses _max-width_ property. _desctop design first_
```
breackpoints{
  "desctop":  1400px,
  "laptop-l": 1200px,
  "tablet-l": 992px,
  "tablet":   768px,
  "mobile-l": 425px,
  "mobile-s": 375px,
}
```

### Uses
```

@include mq(mobile-l) {
  _{styles from 375 to 424px}_
}
@include mq(mobile-s) {
  _{styles from 0 to 374px}_
}
```

