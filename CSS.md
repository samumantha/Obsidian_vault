
## Element selector

```css
p {
	text-align: center;
}
```
-> will align all texts within `<p> </p>` in center

## id selector

```css
#myid {
	text-align: center;
}
```

-> will align all texts which have `id="myid"` in center, id cannot start with a number

## class selector

```css
.myclass {
	text-align: center;
}
```

-> will align all texts which have `class="myclass"` in center; class cannote start with a number

> selectors can also be combined: `p.myclass` -> only counts for `<p class="myclass"> </p>`
> there can also be multiple classes per section `<p class="myclass anotherclass"> </p>`
> selectors can also be grouped:
```css
p , h1 , h2 {
	text-align: center;
}
```
> `*` selects all elements on page

> Multiple style sheets with same selectors: Value from **last read** stylesheet is used, check in which order the stylesheets are linked/defined in html `<head>` -> inline style > external/internal stylesheet > browser default
> the more specific a selector, the higher the rank
> `:root` is pseudo class, targets **everything** within `<html>`

## Comments

```css 
/* here is the comment */
```

## Variables / Properties

* contain specific values to be reused throughout a document
* set using custom property notation (e.g., `--main-color: black;`)  
* accessed using the `var()` function (e.g., `color: var(--main-color);`)
Common usecase to set avriables for complete document:

```css
:root {
  --main-bg-color: brown;
}
```

## Combinators

* ` ` descendant selector, whether it is direct or deeper child
* `>` direct child
* `+` adjacent sibling, immediately after on same level
* `~` general sibling selector

Example: `p > p {}` p and it's direct children p get the styling, not deeper p's!