# markdown-in-html

How do we display markdown content inside of a &lt;details> tag, when the page is deployed on `github pages`?

This fairly niche problem is going to be addressed and solved in this repo!

[Go to the GitHub Pages deployment to see it in action (or not, as the case may be!)](https://frank-ventures.github.io/markdown-in-html/)

---

Apparently you can use an attribute in the `<details>` tag, like so:

```
<details markdown="1">
  <summary>SUMMARY TEXT</summary>

- MARKDOWN CONTENT

- And some more

</details>
```

and it will just work.

---

Lets test!

The following examples will look fine on GitHub when you're viewing the ReadMe, but when you're looking at the deployed Github page the non-attributed version will not display as intended.

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
