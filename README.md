# Második webes workshop

## Érdekesebb részletek

### HTML

[Hasznos tagek](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)

```HTML
    <meta name="theme-color" content="#31343f" />

    <input
      type="text"
      name="search-bar"
      id="search-bar"
      class="shadow"
      spellcheck="false"
      placeholder="Who's your favourite artist?"
      autofocus
    />
```

### CSS

[Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

```CSS
    @import url("https://fonts.googleapis.com/css?family=Open+Sans:400,600&subset=latin-ext");

    :root {
        --primary-color: #5264bf;
        --scroll-color: #ffd6d6;
        --text-color: #31343f;
        --light-text-color: #7a7d8e;
    }

    * {
        margin: 0;
        color: var(--text-color);
        box-sizing: border-box;
        overflow-wrap: break-word;
        word-wrap: break-word;
        word-break: break-word;
    }

    *:focus {
        outline: none;
    }

    html {
        background: linear-gradient(90deg, #fff9e0 0, #ffd6d6 100%);
    }

    .shadow {
        box-shadow: 0 0 5px rgba(0, 0, 0, 0.125);
    }

    .card > .image-container {
        box-shadow: inset 0px 0px 10px 1px rgba(0, 0, 0, 0.25);
        border-radius: 1000px;
        background-size: cover;
        background-repeat: no-repeat;
        background-position: center;
        flex-shrink: 0;
    }

    @media (max-width: 900px) {
        ...
    }

    /* Scrollbar. */
    body::-webkit-scrollbar-track,
    body::-webkit-scrollbar {
        background-color: var(--scroll-color);
        width: 12px;
    }
    body::-webkit-scrollbar-thumb {
        background-color: var(--primary-color);
        border-radius: 1000px;
    }
    /**/

    /* Selections. */
    ::-moz-selection {
        background: var(--primary-color);
        color: white;
    }
    ::selection {
        background: var(--primary-color);
        color: white;
    }
    /**/

    /* Links with interactive underline. */
    .link {
        text-decoration: none;
        position: relative;
        cursor: pointer;
    }
    .link:after {
        content: "";
        height: 5px;
        background-color: var(--primary-color);
        position: absolute;
        left: 0;
        bottom: 0;
        width: 0;
        transition: width 700ms;
        border-radius: 50px;
    }
    .link:hover:after {
        width: 100%;
    }
    /**/
```

### JS

[Reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide)
