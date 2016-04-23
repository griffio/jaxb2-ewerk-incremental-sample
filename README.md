# jaxb2-ewerk-incremental-sample
jaxb2 ewerk plugin incremental compilation using xjc depends/produce

Uses com.ewerk.gradle.plugins:jaxb2-plugin:1.0.2-SNAPSHOT

using local build branch https://github.com/griffio/gradle-plugins/tree/issue%2338

The xjc will only recompile if source schema timestamp is modified.

Changing schema files for bar or foo will recompile only bar or foo.

~~~
src/main/xsd/bar.xsd -> src/generated/example/bar
src/main/xsd/foo.xsd -> src/generated/example/foo
~~~

