Elasticsearch-MySQL-River
=========================

An Elasticsearch river modeled to work like the Solr MySQL import feature

There is an alternative plugin for jdbc connections which you could also try at:
https://github.com/jprante/elasticsearch-river-jdbc

# Building

To build the plugin you need to have maven installed. With that in mind simply check out the project and run "mvn package" in the project directory. The plugin should then be available under target/release as a .zip file.

# Installation

Use the `plugin` command which ships with Elasticsearch to install this River from the GitHub repository. 
Change directory to the Elasticsearch installtion and type:
```
./bin/plugin --install mallocator/Elasticsearch-MySQL-River
```

The plugin needs to be installed on all nodes of the ES cluster.

for more info on plugins check out http://www.elasticsearch.org/guide/reference/modules/plugins.html

# Usage

Check out the `import.sh` script, which is used to initialize the mysql river with all necessary config data.

More info on how to use rivers can be found here: http://www.elasticsearch.org/guide/reference/river/
