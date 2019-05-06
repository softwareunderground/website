Instructions for OS X
=====================

* brew install hugo
* cd softwareunderground
* hugo new site docs
* cd docs
* git submodule add https://github.com/jeblister/kube.git themes/kube
* #echo 'theme = "kube"' >> config.toml
* cp themes/kube/archetypes/* archetypes
* cp -r themes/kube/exampleSite/* .
