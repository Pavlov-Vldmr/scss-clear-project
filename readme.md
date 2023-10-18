# SCSS custom clear project


## Sass start
...
sass --watch scss/index.scss:styles/index.css
...
**box-sizing: border-box**

## Media breacpoints 

@media breackpoints *mixin* uses _max-width_ property. (desctop design first)
...
breackpoints{
  "desctop":  1400px,
  "laptop-l": 1200px,
  "tablet-l": 992px,
  "tablet":   768px,
  "mobile-l": 425px,
  "mobile-s": 375px,
}
...

*example:*
...

@include mq(mobile-l) {
  _{styles from 375 to 424px}_
}
@include mq(mobile-s) {
  _{styles from 0 to 374px}_
}
...

