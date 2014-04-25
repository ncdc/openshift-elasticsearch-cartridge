OpenShift ElasticSearch Cartridge
=================================
Downloadable ElasticSearch cartridge for OpenShift.

To create your scalable ElasticSearch app, run:

    rhc app create <your app name> https://gist.githubusercontent.com/oliviermi/11247443/raw/d75336cc37dac45ad749648afb92ad4a03c92261/manifest.yml-s

**NOTE:** your app currently must be a scalable app or this cartridge will not run.


Adding additional cluster nodes
===============================
To add more nodes to the cluster, simply add more gears:

    rhc cartridge scale -a <your app name> elasticsearch <number of total gears you want>


Plugins
=======
To install ElasticSearch plugins, edit the `plugins.txt` file, commit, and push your changes.


License
=======
This project is licensed under the [Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0.html).
