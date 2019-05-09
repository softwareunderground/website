+++
title = "{{ replace .Name "-" " " | title }}"
date = {{ .Date }}
weight = 20
draft = false
toc = false

description = ""
bref = ""
+++

**Insert Lead paragraph here.**

## New Cool Workflow

{{ range first 10 ( where .Site.RegularPages "Type" "cool" ) }}
* {{ .Title }}
{{ end }}
