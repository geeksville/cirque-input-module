# cirque-input-module experiments

This is a fork of [cirque-input-module](https://github.com/petejohanson/cirque-input-module) with some changes to improve power consumption:

* Put touchpad in shutdown mode when zmk is in deep-sleep
* Only send touch events when there is actually a finger touching the pad (this saves lots of power, because otherwise null touch events were being sent every 10ms)
