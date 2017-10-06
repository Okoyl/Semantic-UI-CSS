# CSS  Distribution with RTL SUPPORT

This repository was taken from [Semantic UI](https://github.com/Semantic-Org/Semantic-UI) repository to provide lightweight CSS only version of Semantic UI.

This package **does not support theming** and includes generated CSS files of the default theme only.

You can view more on Semantic UI at [LearnSemantic.com](http://www.learnsemantic.com) and [Semantic-UI.com](http://www.semantic-ui.com)


# CSS  Distribution MODIFIED:
This distribution was modified in order to accomodate a project with RTL needs.
there are both, RTL and LTR css files,

both:  
`semantic.css` (`semantic.min.css`)       
and   
`semantic.rtl.css` (`semantic.min.rtl.css`)   
are identical other than the fact that semantic.rtl.css was automatically generated using [RTLCSS tool made by Mohammad Younes](https://github.com/MohammadYounes/rtlcss)

Moreover, 3 additional files were generated:   
`common.css` (common.min.css) has whats in common between rtl and ltr versions of the files  
`rtl.css` (rtl.min.css) has only the rtl portion of the files   
`ltr.css` (ltr.min.css) has only the ltr portion of the files   
this allows you to more easily change between rtl and ltr programatically.
please make sure you include `rtl.css` or `ltr.css` first before including `common.css` 
in order for it to work as excpected
in the html page.
## Examples:

### Good for RTL(will work as excpected):
```html
<link rel="stylesheet" type="text/css" href="rtl.css" media="screen" />
<link rel="stylesheet" type="text/css" href="common.css" media="screen" />
```
### Good for LTR(will work as excpected):
```html
<link rel="stylesheet" type="text/css" href="ltr.css" media="screen" />
<link rel="stylesheet" type="text/css" href="common.css" media="screen" />
```
### Bad(will not work as excpected):
```html
<link rel="stylesheet" type="text/css" href="common.css" media="screen" />
<link rel="stylesheet" type="text/css" href="ltr.css" media="screen" />
```
### Bad(will not work as excpected):
```html
<link rel="stylesheet" type="text/css" href="common.css" media="screen" />
<link rel="stylesheet" type="text/css" href="rtl.css" media="screen" />
```
