Instructions for OS X
=====================

* brew install hugo
* cd softwareunderground
* hugo new site docs
* cd docs
* git clone https://github.com/jeblister/kube.git themes
#* echo 'theme = "kube"' >> config.toml
* cp themes/kube/archetypes/* archetypes
* cp -r themes/kube/exampleSite/* .
