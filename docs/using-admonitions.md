---
description: A guide on how to use Docusaurus admonitions to highlight information.
---

# Using Admonitions

Admonitions are a Docusaurus feature that allows you to create styled callout blocks to highlight specific information for the reader. They are useful for drawing attention to notes, tips, warnings, and other important details.

For more in-depth information, you can refer to the [official Docusaurus documentation on Admonitions](https://docusaurus.io/docs/markdown-features/admonitions).

## Basic Usage

To create an admonition, wrap your content in triple colons (`:::`), followed by the admonition type. Docusaurus supports several built-in types:

### Note

Use `note` for standard, neutral information.

```md
:::note
This is a note with some standard information.
:::
```

:::note
This is a note with some standard information.
:::

### Tip

Use `tip` to provide helpful advice or a best practice.

```md
:::tip
This is a tip that offers a helpful piece of advice.
:::
```

:::tip
This is a tip that offers a helpful piece of advice.
:::

### Info

Use `info` for important information that the user should be aware of.

```md
:::info
This is an info block containing important information.
:::
```

:::info
This is an info block containing important information.
:::

### Warning

Use `warning` to caution the user about potential issues or risks.

```md
:::warning
This is a warning. Be careful with the next steps.
:::
```

:::warning
This is a warning. Be careful with the next steps.
:::

### Danger

Use `danger` for critical warnings about actions that could have negative consequences.

```md
:::danger
This is a danger block. Proceeding may cause irreversible damage.
:::
```

:::danger
This is a danger block. Proceeding may cause irreversible damage.
:::

## Customizing Titles

By default, the admonition type is used as the title (e.g., "Note", "Tip"). You can specify a custom title by adding it after the type.

```md
:::info My Custom Title
This admonition has a custom title.
:::
```

:::info My Custom Title
This admonition has a custom title.
:::

You can also use Markdown syntax within your custom title by enclosing it in square brackets.

```md
:::note[A Title **with** some _Markdown_ `syntax`!]
The title of this admonition is formatted with Markdown.
:::
```

:::note[A Title **with** some _Markdown_ `syntax`!]
The title of this admonition is formatted with Markdown.
:::

## Nesting Admonitions

Admonitions can be nested inside one another. To do this, add more colons (`:`) to the wrapper of the parent admonition for each level of nesting.

```md
:::::info Parent Admonition

This is the content of the parent.

::::danger Child Admonition

This is a nested child admonition.

:::tip Deeply Nested Child

This is a deeply nested admonition.

:::

::::

:::::
```

:::::info Parent

Parent content

::::danger Child

Child content

:::tip Deep Child

Deep child content

:::

::::

:::::
