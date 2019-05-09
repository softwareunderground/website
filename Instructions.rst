Instructions for OS X
=====================

* brew install hugo
* hugo new site softwareunderground
* cd softwareunderground
* #hugo new site .
* git submodule add https://github.com/jeblister/kube.git themes/kube
* #echo 'theme = "kube"' >> config.toml
* cp themes/kube/archetypes/* archetypes
* cp -r themes/kube/exampleSite/* .


Getting started with HUGO
=========================

Hugo supports sites with multiple content types and assumes your site will be
organized into `sections <https://gohugo.io/content-management/sections/>`_,
where each section represents the corresponding type.
For our website, sections are, for example, **Gallery** and **Blog**.

Templates
---------
All `templates <https://gohugo.io/templates/introduction/>`_
live in the **layout** folder. Each template gets a data object.
In Hugo, each template is passed a ``Page`` variable.
``.Title`` is one of the elements accessible in the ``Page`` variable.
With ``Page`` being the default scope of a template, the ``Title`` element
in current scope is accessible simply by the dot-prefix notation, ``.Title``.
