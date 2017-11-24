
compton is a lightweight compositor for X that works really well with i3. A compositor adds some eye-candy like transparency and drop-shadows to the windows. But it also do some anti screen tearing magic and such. The compton setup can however be a bit tricky and it all depends on your own preferences and hardware.

The blocks below are more **i3** then hardware related that you might find useful:

``` text
opacity-rule = [ 
  # these transparency rules makes windows in tabs/stacks look good.
  # I only let 5 programs to ever be transparent, and only when they
  # are tiled. Notice the extra rule on qbittorrent, this is necessary 
  # for some Qt applications.
  "0:_NET_WM_STATE@[0]:32a = '_NET_WM_STATE_HIDDEN'",
  "0:_NET_WM_STATE@[1]:32a = '_NET_WM_STATE_HIDDEN'",
  "0:_NET_WM_STATE@[2]:32a = '_NET_WM_STATE_HIDDEN'",
  "0:_NET_WM_STATE@[3]:32a = '_NET_WM_STATE_HIDDEN'",
  "0:_NET_WM_STATE@[4]:32a = '_NET_WM_STATE_HIDDEN'",
  "90:class_g = 'Sublime_text' && !_NET_WM_STATE@:32a && !I3_FLOATING_WINDOW@:c",
  "90:class_g = 'URxvt' && !_NET_WM_STATE@:32a && !I3_FLOATING_WINDOW@:c",
  "90:class_g = 'qBittorrent' && !I3_FLOATING_WINDOW@:c && !_NET_WM_STATE@[2]:32a",
  "90:class_g = 'Klavaro' && !_NET_WM_STATE@:32a && !I3_FLOATING_WINDOW@:c",
  # its important that the last rule doesn't have a comma ',' at the
  # EOL (end of line)
  "90:class_g = 'Spacefm' && !_NET_WM_STATE@:32a && !I3_FLOATING_WINDOW@:c"
];

shadow-exclude = [
    # the first two rules is a dirt-hack to make my bar not have a shadow.
    "x<=3 && x2>= 1000 && y <= 30 && y2 >=750",
    "x = 0 && y = 0 && override_redirect = true",
    # make sure tiled windows doesn't have a shadow, might be desired when
    # using gaps.
    "!I3_FLOATING_WINDOW@:c",
    # these rules makes sure the window title bar doesn't have a shadow.
    "class_g = 'i3-frame'",
    "_GTK_FRAME_EXTENTS@:c"
    "name = 'Notification'",
    "class_g = 'Conky'"
];
```

And this is the full `compton.conf` file:

