
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

## Comments

```
/* here is the comment */
```
