+++
description = "Get value of site params variables in your page"
title = "Site param"
+++

`siteparam` shortcode is used to help you print values of site params.

For instance, in this current site, the `editURL` variable is used in `config.toml`

```toml
[params]
  editURL = "https://github.com/McShelby/hugo-theme-relearn/edit/main/exampleSite/content/"
```

Use the `siteparam` shortcode to display its value.

```go
`editURL` Value : {{%/* siteparam "editURL" */%}}
```

is displayed as

`editURL` Value : {{% siteparam "editURL" %}}