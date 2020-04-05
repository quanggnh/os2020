Satellite
=========

1.  Two-way only:

-   Sending and receiving data through VSAT
    (very-small-apeture-terminal,bascially a ground station with a small
    dish antenna (0.75 to 1.2 m,4 kbit/s to 16 Mbit/s) to
    telecommunication port (satellite ground station connecting
    satellite network with Internet) then to Internet +Need strict setup
    -\> hard to use on moving vehicle
-   Both single channel per carrier or time division multiple access (1
    channel divided to many time slot) +Example: SES Broadband operating
    in Ku band (12 to 18 GHz) xBandwidth: Usually restrictive time-based
    based on pay,uplink for shared time divisino multiple access
-   A shared download carrier: 1 to 40 Mbit/s for 100 to 4000 end users
    +May use telephone modem,may use modem channel when prio for latency
    \> bandwith 
xPortable: Use self-contained box point to satellite,not
			too precise,very expensive (5 -\> 7 dollar per megabyte)

x Satellite phone:Low bandwith -\> slow to browse net,useful for
sending email. Having omnidirectional antennas -\> don't need alignment

2.  One way receive terrestrial transmit

-   Use common dial-up internet access: upstream through telephone
    modem, downstream through satellite 
-	Consist of high speed Internet connection + satellite uplink
-   Data is encrypted when sent to satellite so not everyone with
    satellite can access +Use nonstandard IP stacks to address latency
    problem
-   Upload speed limited by the user's modem,download speed can be fast:
    The modem only served as control channel for packet acknowledgement
	still generally slower than terrestrial broadband method
-   Half latency: Half as 2-way as only downstream data is transmit by
    satellite, still high as expected


3.  One way multicast: +Used for IP multicast-based data,audio,video
    distribution

-   Will not correctly with 1 way access (I.e Internet content but can't
    fully interact with,simillar to TV,radio content)

