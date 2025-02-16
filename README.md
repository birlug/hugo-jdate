## Hugo JDate
hugo jalali date you were looking for.

### Install as a Hugo Module
add this to your TOML config file:
```toml
[module]
  [[module.imports]]
    path = "github.com/birlug/hugo-jdate"
```

read more about hugo modules [here](https://gohugo.io/hugo-modules/use-modules/).

### Usage
imagine your `MD` file looks like this:
```md
---
title: "example title"
date: 2019-09-08
---
```

then `hugo-jdate` partial can be used like this in your html files:
```html
<a>{{ .Title }} - {{ partial "jDate.html" .Params.Date }}</a>
```
