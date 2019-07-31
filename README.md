# ros_logrotate

Have you ever noticed that your ROS log folder grows indefinitely? In production applications, this can generate gigabytes of data full of old and useless log files. 

This logrotate script allows you to control the size of your log files and make your ROS log folder cleaner. It will compress old folders and remove them after some days. This script is configuarable and you can set the number of days you want to keep files. Plus, it will also clean log files from terminal calls, like rostopic pub or rosservice call.

# Usage 

Install logrotate, if you don't have it. Most of Linux distribuitions come with it by default, but you can install it by running:

```
sudo apt-get install logrotate
```
Make sure also you have cron installed if you want this logrotate script to run regularly.

Then, please read the logrotate_ros file. It has some comments and you might need to change some stuff yourself. After doing your changes, drop this file at /etc/logrotate.d. Everything should work fine now.

# Problems?

Feel free to fill an issue ticket [here](https://github.com/lucascoelhof/ros_logrotate/issues)
