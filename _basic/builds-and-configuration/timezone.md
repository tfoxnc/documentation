---
title: Setting Timezone
menus:
  basic/builds:
    title: Setting Timezone
    weight: 10
tags:
  - timezone
categories:
  - Builds and Configuration
  - Configuration
redirect_from:
  - /basic/getting-started/timezone/
---

* include a table of contents
{:toc}

## Default Timezone On CodeShip Basic

The default timezone on CodeShip's test VMs is `UTC +00:00` or `Etc/UTC`.

## Setting A Custom Timezone

You can set a custom timezone with a specific environment variable, and there are two ways to set this value. You can either use your [project's environment variables UI]({{ site.baseurl }}{% link _basic/builds-and-configuration/set-environment-variables.md %}) or you can set it via a custom script in your [setup commands]({{ site.baseurl }}{% link _basic/quickstart/getting-started.md %})

You simply need to set the value `TZ` to the timezone of your choice. If using your own script, you will run something like:

```shell
export TZ='America/New_York'
```

You can see the [full list of valid TZ values here](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones).
