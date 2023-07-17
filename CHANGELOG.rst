^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package greenzie_ntrip_client
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

1.2.4 (2023-07-17)
------------------
* Fixed Bug with Building Python Debian

1.2.3 (2023-06-26)
------------------
* Changed the default NMEA Max Message Length to 84

1.2.2 (2023-03-14)
------------------
* Adds ability to publish raw RTCM into uint8 multiarray
* Added respawn to the node
* Changed Default NMEA Max Message Length

1.2.0 (2022-08-11)
------------------
* Adds the ability to configure the NTRIP client to connect using SSL (`#23 <https://github.com/LORD-MicroStrain/ntrip_client/issues/23>`_)
* ROS automatic reconnect (`#18 <https://github.com/LORD-MicroStrain/ntrip_client/issues/18>`_)
  * Adds ability to reconnect to ROS
  * Allows the timeouts and other parameters to be modified via the launch file
  * Moves optional config out of constructor, and declares constnats in class definition
* Contributors: Rob

1.1.0 (2022-04-22)
------------------
* ROS Ntrip Version Configuration (`#8 <https://github.com/LORD-MicroStrain/ntrip_client/issues/8>`_)
  * No longer sends Ntrip-Version header if not specified
  * Adds some hopefully helpful debug logging
  * Properly handles responses that have both a failure response and success response
  * Adds ability to print debug logs via launch parameter
* Contributors: robbiefish

1.0.1 (2022-02-10)
------------------
* Checks if there is a * character in the string before parsing fully
* Contributors: robbiefish

1.0.0 (2021-12-08)
------------------
* Initial implementation of ROS NTRIP client
* Adds ability to cache packets if they do contain some of a mesage but not the whole thing
* Contributors: drobb257, nathanmillerparker, robbiefish
