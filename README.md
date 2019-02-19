# 3DR Solo Quadcopter Digital Twin for GymFC

This digital twin is meant to serve as an example for the new
[GymFC](https://github.com/wil3/gymfc) architecture used in versions v0.2+.  

It uses a port of the [PX4 SITL Gazebo plugins](https://github.com/wil3/gymfc-aircraft-plugins) and 
the PX4 SITL Solo models. The Iris quadcopter initially used by GymFC has not
been ported to the new plugins, thus the Solo model is being substituted as an
example.

The new GymFC architecture allows for each digital twin to be version
controlled. 

Note: This is all very experimental, the PX4 motor models are still in
development. We require additional documentation and validation on the affects
of these models.

## Configuration File

Each digital twin is defined by its configuration file. 

## Instructions 

1) Clone and build the [GymFC Aircraft Plugins](https://github.com/wil3/gymfc-aircraft-plugins) repo.
2) Rename `solo.json.template` to `solo.json`.
3) Set `model_dir` to "<path to this repo>/models"  
4) Set `model` to "<path to this repo>/models/solo/model.sdf"
3) Set `plugin_dir` to "<path to GymFC Aircraft Plugins repo>/build"
