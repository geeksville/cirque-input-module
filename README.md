# cirque-input-module (tweaked)

This is a fork of the original [cirque-input-module](https://github.com/petejohanson/cirque-input-module) with the following (IMO) improvements:

* Place chip into shutdown mode anytime ZMK is in deep-sleep (this saves lots of power - see the commit for details)
* Optionally operate the chip in absolute mode, so we can generate BTN_TOUCH events for finger on/off trackpad
* Add an abs-rel mode that generates relative move events, but still generate touch events (for automatic layer switching)

For details on these changes and discussion see the pull-requests sent upstream.

Thanks to Pete Johanson for the original driver!