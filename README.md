# ros_logrotate

Have you ever noticed that your ROS log folder grows indefinitely? In production applications, this can generate gigabytes of data full of old and useless log files. 

This logrotate script allows you to control the size of your log files and make your ROS log folder cleaner. It will compress old folders and remove them after some days. This script is configuarable and you can set the number of days you want to keep files. Plus, it will also clean log files from terminal calls, like rostopic pub or rosservice call.

