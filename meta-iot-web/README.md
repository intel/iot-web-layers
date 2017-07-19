meta-iot-web
------------

Yocto layer for the IoT web components including Node.js, IoT REST API Server, iotivity-node, etc

Dependencies
------------

This layer depends on:

    meta: git://git.openembedded.org/openembedded-core
    meta-oic: git://git.yoctoproject.org/meta-oic

Recipes in meta-iot-web
-----------------------

    recipes-web: Recipes for the iotivity-node and iot-rest-api-server
    recipes-devtools: Recipes for the Node.js and JavaScript Robotics
                      Programming Framework modules - johnny-five and
                      galileo-io
    recipes-smarthome: Recipes for the IoT to Cloud Smart Home demo

Adding the meta-iot-web layer to your build
-------------------------------------------

In order to use this layer, you need to make the build system aware of
it.

Assuming the meta-iot-web layer exists at the top-level of your
yocto build tree, you can add it to the build system by adding the
location of the meta-iot-web layer to bblayers.conf, along with any
other layers needed. e.g.:

```shell
  BBLAYERS ?= " \
    /path/to/oe-core/meta \
    /path/to/layer/meta-oic \
    /path/to/layer/meta-iot-web \
    "
```

Submitting Patches
------------------

Please submit patches via Github pull requests in
https://github.com/intel/iot-web-layers
