# Zola-Paper Blog
A clean blog theme based on [Zola-Paper](https://github.com/schoenenberg/zola-paper).

## Installation

The easiest way to install this theme is to either clone it ...

```bash
git clone https://github.com/light-traveller/zola-paper-blog.git themes/zola-paper-blog
```

... or to use it as a submodule.

```bash
git submodule add https://github.com/light-traveller/zola-paper-blog.git themes/zola-paper-blog
```

Either way, you will have to enable the theme in your `config.toml`.

```toml
theme = "zola-paper-blog"
```

## Open Graph Integration

This theme has an integration of Open Graph *meta* tags. These are set based on context and available information. See the following example:

```markdown
+++
title = "Lorem ipsum!"

[extra]
author = "John Doe"
author_url = "https://www.facebook.com/example.profile.3"
banner_path = "default-banner"

[taxonomies]
tags = ["rust", "zola", "blog"]
+++

Lorem ipsum dolor sit amet, consectetur adipiscing elit.
<!-- more -->
Ut luctus dolor ut tortor hendrerit, sed hendrerit augue scelerisque. Suspendisse quis sodales dui, at tempus ante. Nulla at tempor metus. Aliquam vitae rutrum diam. Curabitur iaculis massa dui, quis varius nulla finibus a. Praesent eu blandit justo. Suspendisse pharetra, arcu in rhoncus rutrum, magna magna viverra erat...
```

- The only required attributes of the `extra` section is `author`. All other attributes are optional.
- The path for the `banner_path` attribute has to be relative to the content directory.
