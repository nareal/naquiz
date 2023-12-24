# naquiz extension for Quarto

![GitHub Action Status](https://img.shields.io/github/actions/workflow/status/nareal/naquiz/publish.yml)

The extension enables adding multiple choice questions when using a Quarto HTML documents or Quarto revealjs presentation. It also adds [Alpine.js](https://alpinejs.dev/) javascript framework to the document.

## Installing

To install the extension with the template do:

```bash
quarto use template nareal/naquiz
```


To install the extension without the template do:

```bash
quarto add nareal/naquiz
```

This will install the extension under the `_extensions` subdirectory.
If you're using version control, you will want to check in this directory.


To update the extension use:

```bash
quarto update extension nareal/naquiz
```

and to remove it:

```bash
quarto remove extension nareal/naquiz
```

## Using

To use the extension simply add it as a filter to the YAML header of the quarto document, for example:

```default
---
title: "naquiz Example"
filters:
  - naquiz
---

:::::{.question}
Bill Gates was the founder of:

::::{.choices}

:::{.choice}
Apple
:::  

:::{.choice .correct-choice}
Microsoft
:::

:::{.choice}
Facebook  
:::

:::{.choice}
Google   
:::

::::
:::::
```

## Example

Here is the source code with usage examples: [example.qmd](example.qmd) and the [rendered HTML page](https://nareal.github.io/naquiz/example.html).

Here is the source code for an example of usage with revealjs presentation: [example_presentation.qmd](example_presentation.qmd) and the [rendered HTML page](https://nareal.github.io/naquiz/example_presentation.html). 
