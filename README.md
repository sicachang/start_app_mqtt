Eclipse Mosquitto
=================

Mosquitto is an open source implementation of a server for version 5.0, 3.1.1,
and 3.1 of the MQTT protocol. It also includes a C and C++ client library, and
the `mosquitto_pub` and `mosquitto_sub` utilities for publishing and
subscribing.

## Installing

See <https://mosquitto.org/download/> for details on installing binaries for
various platforms.

## Quick start

If you have installed a binary package the broker should have been started
automatically. If not, it can be started with a basic configuration:

    mosquitto

Then use `mosquitto_sub` to subscribe to a topic:

    mosquitto_sub -t 'test/topic' -v

And to publish a message:

    mosquitto_pub -t 'test/topic' -m 'hello world'


## Credits

Mosquitto was written by Roger Light <roger@atchoo.org>

Master: [![Travis Build Status (master)](https://travis-ci.org/eclipse/mosquitto.svg?branch=master)](https://travis-ci.org/eclipse/mosquitto)
Develop: [![Travis Build Status (develop)](https://travis-ci.org/eclipse/mosquitto.svg?branch=develop)](https://travis-ci.org/eclipse/mosquitto)
Fixes: [![Travis Build Status (fixes)](https://travis-ci.org/eclipse/mosquitto.svg?branch=fixes)](https://travis-ci.org/eclipse/mosquitto)
