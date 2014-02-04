OpenShift ElasticSearch Cartridge
=================================
Downloadable ElasticSearch cartridge for OpenShift.

To create your scalable ElasticSearch app, run:

```
rhc app-create --scaling es https://reflector-getupcloud.getup.io/github/ncdc/openshift-elasticsearch-cartridge
```

You don't want a nonscalable one, right?

To add more ES nodes to the cluster, simply add more gears:

```
rhc cartridge-scale elasticsearch --app es --min 3
````

That will add 2 more gears to your app.

Plugins
=======

To install plugins, edit repo file `plugins.txt` and read the instructions.

License
=======
This project is licensed under the [Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0.html).
