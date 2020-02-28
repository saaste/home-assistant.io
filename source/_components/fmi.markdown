---
layout: page
title: "Finnish Meteorological Institute"
description: "How to integrate FMI within Home Assistant."
date: 2019-02-28 22:46
sidebar: true
comments: false
sharing: true
footer: true
logo: fmi.png
ha_category: Weather
ha_release: 0.106
ha_iot_class: Cloud Polling
---

The `fmi` platform uses [Finnish Meteorological Institute](https://en.ilmatieteenlaitos.fi/) as a source for current
meteorological data. The weather forecast is delivered by the Finnish Meteorological Institute (FMI).

## {% linkable_title Configuration %}

To add FMI to your installation, add the following to your `configuration.yaml` file:

```yaml
# Example configuration.yaml entry
weather:
  - platform: fmi
```

{% configuration %}
name:
  description: Additional name for the sensors.
  required: false
  type: string
  default: FMI
latitude:
  description: Manually specify latitude. By default the value will be taken from the Home Assistant configuration.
  required: false
  type: float
  default: Provided by Home Assistant configuration
longitude:
  description: Manually specify longitude. By default the value will be taken from the Home Assistant configuration.
  required: false
  type: float
  default: Provided by Home Assistant configuration
{% endconfiguration %}

