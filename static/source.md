### Movement

Use `space` key to navigate to the next slide in the order intended by the creator or do as you please with the arrow keys.

---

## Nested Slides

Reveal.js allows you to have nested slides, these nested slides allow one to have slides that move to the right as well as down.\
Press `esc` key to have a top down view of all slides.

If you want to insert a vertical slide, use the vertical divider in the markdown.\
`--` is a vertical divider, which makes nested slides.

--

Example of Nested Slide.

--
If you want to go to the next slide use the horizontal divider.\
`---` is for horizontal divider.

---

### Math Mode

You can use inline math mode with `$<content>$`` and block math mode by
```
$$
<content>
$$
```

--

#### Inline Math Expression

`$\sin(\alpha) + \frac{2}{3}`\
renders as\
$\sin(\alpha) + \frac{2}{3}$

--

#### Block Math Expression

```
$$
e^{x} = \sum^{\infty}_{i=0} \frac{x^{i}}{i!}
$$
```
renders as\
$$
e^{x} = \sum^{\infty}_{i=0} \frac{x^{i}}{i!}
$$

--

By default this template uses KaTeX to render TeX, please check out KaTeX documentation for things you can and can not do.

---

### Code

Reveal.js uses Marked.js behind the scenes for the markdown.\
This allows us to do very cool stuff code diplaying stuff.\
We also get capability to highlight the code we right with relatively less pain.

--

#### Example

```js
console.log("Hello World");
a = 2;
b = false;
console.log(b + a);
```
--

#### Animation in between lines

```js[732: 1|2-3|4]
console.log("Hello World");
a = 2;
b = false;
console.log(b + a);
```

-- 

Please check the source file for more information on how to achieve thes effects.