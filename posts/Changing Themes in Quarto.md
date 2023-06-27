---
format:
  html:
    css: css/quarto.css
---

# Change Themes in Quarto

*Quarto provides a selection of attractive themes that can alter the look and feel of your documents. Let's dive into
how to switch themes in Quarto and take a look at the default themes available.*

**Changing Themes in Quarto:**

Themes in Quarto are set in the YAML metadata at the beginning of your document. You can specify the theme using
the `html:` field for HTML documents. Here's an example:

```yaml
---
title: "My Document"
html:
  theme:
    name: "cerulean"
---
```

In this example, we've set the theme of our document to "cerulean". Simply replace "cerulean" with the name of the theme
you'd like to use.

Absolutely, adjusting the theme for all documents in a project is a useful technique when maintaining consistent
styling.

## **Setting a Global Theme in Quarto:**

Quarto allows you to set a global theme for all the documents in your project using the `_quarto.yml` configuration
file. This can be particularly handy when you want all your documents to maintain a consistent look and feel.

Here's how you can do it:

1. Locate or create the `_quarto.yml` file in your project's root directory.
2. Set the `html:` field and the `theme:` field as shown in the following example:

```yaml
# _quarto.yml
html:
  theme:
    name: "cerulean"
```

In this example, we've set the theme for all HTML documents in our project to "cerulean". Simply replace "cerulean" with
the name of the theme you'd like to use for your documents.

Remember, if a theme is specified in the YAML metadata of a specific document, it will override the global theme set in
the `_quarto.yml` file.

## **Default Themes Available:**

Quarto uses the Bootswatch themes, which provide several different styles to choose from. As of my knowledge cutoff in
September 2021, the following themes are available:

1. Default
2. Cerulean
3. Cosmo
4. Flatly
5. Journal
6. Litera
7. Lumen
8. Lux
9. Materia
10. Minty
11. Pulse
12. Sandstone
13. Simplex
14. Sketchy
15. Slate
16. Solar
17. Spacelab
18. Superhero
19. United
20. Yeti

To apply any of these themes, replace "cerulean" in the YAML metadata with the name of your chosen theme.

Changing the theme of your document is a simple yet powerful way to enhance its visual appeal. Explore the different
themes available to find one that suits your content and audience!

