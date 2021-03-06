Change log
==========

1.4.0 (2018-05-16)
==================

* API changes:
  * None
* Deprecated features:
  * None
* New features:
  * cisst_ros_bridge:
    * Added support for tf2 from read command
    * Added options for queue size and latch for publishers (important for events)
    * Better time stamping and setting valid flag in conversion from ROS to cisst
    * Export moving/reference frame from cisst to ROS tf2, twist and tranform
    * mtsIntervalStatistics: added custom message and publishes statistics from ros bridge task
* Bug fixes:
  * None

1.3.0 (2017-11-07)
==================

* API changes:
  * None
* Deprecated features:
  * None
* New features:
  * cisst_msgs: added StringStamped
  * cisst_ros_bridge: added more data conversion methods:
    * Joy from prmInputData
    * mtsMessage to ROS messages
    * More twist and angular velocities
    * mtsDoubleVec to Float64MultiArray
    * mtsIntervalStatistics custom message
  * cisst_ros_bridge:
    * use std::copy instead of loops with random access
    * standardized error message when creating interfaces
    * factorized conversion methods when possible
    * started to use header.frame when a name is available in cisst
* Bug fixes:
  * None


1.2.0 (2016-08-30)
==================

* API changes:
  * None
* Deprecated features:
  * None
* New features:
  * cisst_msgs: added StringStamped
  * cisst_ros_bridge: added more data conversion methods:
    * Joy from event button pressed
    * Float64MultiArray from dynamic matrix
    * PointCloud from std::vector<vct3>
  * cisst_ros_bridge: use cisstMultiTask timestamp to set ROS time for messages with header
* Bug fixes:
  * gcc: minor fixes to avoid warnings


1.1.0 (2016-01-08)
==================

* API changes:
  * None
* Deprecated features:
  * None
* New features:
  * cisst_ros_bridge: Added more data conversion methods (BoolStamped)
* Bug fixes:
  * None


1.0.1 (2015-10-18)
==================

* Change log file created
* API changes:
  * None
* Deprecated features:
  * None
* New features:
  * cisst_ros_bridge: Added prmStateJoint data type
  * cisst_ros_bridge: Added support to convert events with std::string to ROS log messages
  * cisst_ros_bridge: Added more data conversion methods (int32, mtsFrm4x4)
* Bug fixes:
  * cisst_ros_bridge: Only read/convert if there are active subscribers
