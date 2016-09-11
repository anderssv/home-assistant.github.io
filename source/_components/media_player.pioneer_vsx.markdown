---
layout: page
title: "Pioneer Network Receivers (VSX range)"
description: "Instructions on how to integrate a Pioneer Network Receivers into Home Assistant."
date: 2016-08-11 08:00
sidebar: true
comments: false
sharing: true
footer: true
logo: pioneer.png
ha_category: Media Player
featured: false
ha_release: 0.29
---

The `pioneer_vsx` platform allows you to control Pioneer Network Receivers. It has been tested with
VSX 510k. Please update if you test with others.

*WARNING:* There is a bug in the VSX receivers that makes them stop responding. To reset the reciver,
you will need to unplug the power completely. We're sorry, there is nothing we can do to fix this.

To add a Pioneer receiver to your installation, add the following to your `configuration.yaml` file:

```yaml
# Example configuration.yaml entry
media_player:
  platform: pioneer_vsx
  host: 192.168.0.10
  name: Living receiver
```

Configuration variables:

- **host** (*Required*): The IP of the Pioneer device,  eg. `192.168.0.10`
- **name** (*Optional*): The name you would like to give to the receiver.
- **port** (*Optional*): The port that your reciver respons to. Will default to 8102 if not specified.
