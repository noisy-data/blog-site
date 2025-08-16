---
title: 'Under Construction'
published: 2025-08-16
draft: false
featured: true
tags: ['general']
toc: true
description:  Placeholder first post while the site is under construction...
---




## Theming

> Use your favorite editor theme for your blog!

Theming for the website comes from builtin Shiki themes found in Expressive Code. You can view them [here](https://expressive-code.com/guides/themes/#available-themes). A website can have one or more themes, defined in `src/site.config.ts`. There are three theming modes to choose from:

1. `single`: Choose a single theme for the website. Simple.
2. `light-dark-auto`: Choose two themes for the website to use for light and dark mode. The header will include a button for toggling between light/dark/auto. For example, you could choose `github-dark` and `github-light` with a default of `"auto"` and the user's experience will match their operating system theme straight away.
3. `select`: Choose two or more themes for the website and include a button in the header to change between any of these themes. You could include as many Shiki themes from Expressive Code as you like. Allow users to find their favorite theme!

> When the user changes the theme, their preference is stored in `localStorage` to persist across page navigation.

## Code Blocks

Let's look at some code block styles:

```python
def hello_world():
    print("Hello, world!")

hello_world()
```

```python title="hello.py"
def hello_world():
    print("Hello, world!")

hello_world()
```

```shell
python hello.py
```

Also some inline code: `1 + 2 = 3`. Or maybe even `(= (+ 1 2) 3)`.

See the [Expressive Code Docs](https://expressive-code.com/key-features/syntax-highlighting/) for more information on available features like wrapping text, line highlighting, diffs, etc.

## Basic Markdown Elements

- List item 1
- List item 2

**Bold text**

_Italic text_

~~Strikethrough text~~

[Link](https://www.example.com)

> In life, as in art, some endings are bittersweet. Especially when it comes to love. Sometimes fate throws two lovers together only to rip them apart. Sometimes the hero finally makes the right choice but the timing is all wrong. And, as they say, timing is everything.
>
> \- Gossip Girl

| Name    | Age | City        |
| ------- | --- | ----------- |
| Alice   | 30  | New York    |
| Bob     | 25  | Los Angeles |
| Charlie | 35  | Chicago     |

---

## Admonitions

```md title="Admonition example in markdown"
:::note
testing123
:::
```

:::note
testing123
:::

:::tip
testing123
:::

:::important
testing123
:::

:::caution
testing123
:::

:::warning
testing123
:::
