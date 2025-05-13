# markdown-in-html

How to display a markdown list in a &lt;details> tag?

[Go to the GitHub Pages deployment to see it in action (or not, as the case may be!)](https://frank-ventures.github.io/markdown-in-html/)

Apparently you can use an attribute like so:

```html
<details markdown="1">
  <summary>SUMMARY TEXT</summary>

  - MARKDOWN CONTENT - And some more
</details>
```

and it will just work.

Lets test!

## Lists

### With attribute

<details markdown="1">

 <summary>SUMMARY TEXT</summary>

- MARKDOWN CONTENT

- And some more

</details>

### Without attribute

<details>

 <summary>SUMMARY TEXT</summary>

- MARKDOWN CONTENT

- And some more

</details>

## Code Blocks

### With attribute

<details markdown="1">

 <summary>Open me to see CSS</summary>

```css
.my-awesome-css {
  background-colour: khaki;
}
```

</details>

### Without attribute

<details>

 <summary>Open me to see CSS</summary>

```css
.my-awesome-css {
  background-colour: khaki;
}
```

</details>
