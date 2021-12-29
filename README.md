# GIST-KU msgs

ROS messages for GIST-KU unstructured assembly project


## gist_ku_msg/AssemblyOrder.msg

```
import rospy
from gist_ku_msgs.msg import AssemblyOrder
rospy.init_node("test")
msg = rospy.wait_for_message("/unstructured/assembly_order", AssemblyOrder)
print(msg.assembly_order)
>> ["usb", "power", "hdmi"]
```

## gist_ku_msg/PhaseDetection.msg

```
import rospy
from gist_ku_msgs.msg import PhaseDetection
rospy.init_node("test")
msg = rospy.wait_for_message("/unstructured/phase_detection", PhaseDetection)
print(msg.phase_name)
>>> cpu
>>> cooler
>>> ram
>>> ssd
>>> bolt
```
