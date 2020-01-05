# hass-config-template

A basic starting template for Home Assistant

## Sections

* How to Use
* Home Assistant Files (config/)
  * [configuration.yaml](#configuration.yaml)
  * [secrets.yaml](#secrets.yaml)
  * packages/

## How to Use

TL;DR copy the `config/` folder into your Home Assistant location and tweak to taste.

The `config/` folder contains a working configuration setup of Home Assistant. It is very close to a fresh install, but has organization configured to allow easy updates and organization.

If you are using hass.io (or hassOS) you will copy the contents of this config folder `config/` into the Home Assistant config folder `/config/`. Look through the sections below to see what you should change in the configs to personalize them for your location.

## Home Assistant Files (config/)

These are the configuration files (and folders) that are used to configure Home Assistant. Minimally you need a `configuration.yaml` file and you should have a `secrets.yaml` file for separating out passwords and keys.

### configuration.yaml

This file is the primary file Home Assistant looks at. Within this file, you can link in other files for Home Assistant to pull configuration from.

There are several things you will most likely want to change for your installation:
* latitude (in `secrets.yaml`)
* longitude (in `secrets.yaml`)
* elevation
* time_zone
* unit_system
* name (if you want your "Home" zone to be called something else)


### secrets.yaml

This file is where you should place all private/secret information. This can include:

* Passwords
* API Keys
* Locations
* Names
* Anything you would not want others to know

One main use of the `secrets.yaml` file is when backing up or sharing your configuration. You can exclude the `secrets.yaml`
 file and then openly share the rest of your configuration.

> NOTE: All values in the given `secrets.yaml` file are examples and are not valid/usable.
