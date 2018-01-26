# ros_unicode_message_transfer
This is a simple talker listener in ros.
ros by default does not support message transfer in unicode but this project shows a way around.

ROS only supports ASCII characters for message transfering. Here, what I have done is:
In talker: Encode the unicode string in utf-8
In listener: Collect the string from data attribute and then decode the utf-8 to unicode.
One important point is to set utf-8 as default encoding format.
