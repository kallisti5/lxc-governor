![](http://f.cl.ly/items/2V1L3Y0y1S1K2z392x3n/Screen%20Shot%202012-09-17%20at%2012.09.56%20PM.png)

The `lxc-frontend` is a small Sinatra app which was created to speed-up the monitoring and management of LXC containers. You can start/stop/restart any container, change the container config and network interfaces.

#Requirements:
* the user which runs the Sinatra app should have sudo permissions without a password prompt
* LXC containers configs should have a write permission under the app. It can be fixed by assigning the `a+w` rule to container config and rootfs/network/interfaces files

#How to use

1. Download the app: `git clone ...`
2. Install them gems: `bundle install`
3. Boot'er up: bundle exec rackup -d -p 4567 config.ru
4. PROFIT!
