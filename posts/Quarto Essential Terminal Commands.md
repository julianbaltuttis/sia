# Essential Terminal Commands in Quarto

*Learn Basic Terminal Commands for Launching Quarto Websites.*

Quarto is a powerful open-source scientific and technical document processing system. To leverage Quarto effectively,
it's important to familiarize yourself with its essential terminal commands. Here's an overview of the most commonly
used commands:

**1. `quarto render`:**

This command is used to generate output documents. By default, it will produce an output for every input document in the
project. You can specify a single document or a list of documents to render.

```bash
# Render all documents
quarto render

# Render specific document
quarto render document.qmd
```

**2. `quarto preview`:**

This command is used to preview your documents in a web server. As you make changes to your files, the server
automatically re-renders your documents.

```bash
quarto preview
```

**3. `quarto watch`:**

Similar to `quarto serve`, this command monitors your documents for changes. Instead of serving them in a web server, it
simply re-renders the documents.

```bash
quarto watch
```

**4. `quarto install`:**

This command ensures that all the dependencies for your project are installed. It's particularly useful when you clone a
project from a version control system.

```bash
quarto install
```

**5. `quarto check`:**

This command verifies that your project configuration and environment are correctly set up. It checks things like
project configuration, required software, and document dependencies.

```bash
quarto check
```

**6. `quarto clean`:**

This command removes all generated output files and any cached metadata associated with them.

```bash
quarto clean
```

Mastering these essential Quarto commands will help you navigate and manipulate your Quarto projects more effectively.
For a more in-depth understanding, refer to the official [Quarto CLI documentation](https://quarto.org/docs/cli.html).

