---
layout: full
homepage: true
disable_anchors: true
description: docs for small projects.
---

This sets up the simple themed docs for a small project.

Actually this site is using the theme.

<div class="row">
<div class="col-lg-6" markdown="1">

## Installation
{:.mt-lg-0}

We are using the `dotnet cli` support for templates, so you will need to install `.NET 5` (or `.NET Core 3.1`)

### nuget Template

Add our nuget source

```sh
dotnet nuget add source https://nuget.pkg.github.com/dbones-labs/index.json -n gh-dbones-labs -u YOUR_USER_NAME -p GH_TOKEN [--store-password-in-clear-text]
```

Install the template

```sh
dotnet new -i DBones.Template.Docs.Simple --nuget-source gh-dbones-labs
```

### Docs Branch

this is one possible way


1. Add a branch called `docs`
2. Add the template to the `docs` branch


```sh
dotnet new simple-doc --organisation-name "dbones-labs" --project-name "template-docs-simple"
```

3. update the content

</div>
<div class="col-lg-6" markdown="1">

## Github
{:.mt-lg-0}

### Pages

1. Settings > Github Pages
2. Set the Github pages to `docs`


</div>
</div>
