1	M U M B L E 
2 
 
3  A voicechat utility for gamers 
4 
 
5       http://mumble.info/ 
6 
 
7       #mumble on freenode 
8 
 
9 Mumble is a voicechat program for gamers written on top of Qt and Opus. 
10 
 
11 There are two modules in Mumble; the client (mumble) and the server 
12 (murmur). The client works on Win32/64, Linux and Mac OS X, while the 
13 server should work on anything Qt can be installed on. 
14 
 
15 Note that when we say Win32, we mean Windows XP or newer. 
16 
 
17 Running Mumble 
18 ============== 
19 
 
20 On Windows, after installation, you should have a new Mumble folder in your 
21 Start Menu, from which you can start Mumble. 
22 
 
23 On Mac OS X, to install Mumble, drag the application from the downloaded 
24 disk image into your /Applications folder. 
25 
 
26 Once Mumble is launched, you need a server to connect to. Either create your 
27 own or join a friend's. 
28 
 
29 Running Murmur on Unix-like systems 
30 =================================== 
31 
 
32 Murmur should be run from the command line, so start a shell (command prompt) 
33 and go to wherever you installed Mumble. Run murmur as 
34 
 
35 murmurd [-supw <password>] [-ini <inifile>] [-fg] [v] 
36 
 
37 -supw   Set new password for the user SuperUser, which is hardcoded to 
38         bypass ACLs. Keep this password safe. Until you set a password, 
39         the SuperUser is disabled. If you use this option, murmur will 
40         set the password in the database and then exit. 
41 
 
42 -ini    Use a inifile other than murmur.ini, use this to run several instances 
43         of murmur from the same directory. Make sure each instance is using 
44         a separate database. 
45 
 
46 -fg     Run in the foreground, logging to standard output. 
47 
 
48 -v      More verbose logging. 
49 
 
50 Running Murmur on Mac OS X 
51 ========================== 
52 
 
53 Murmur is distributed seperately from the Mumble client on Mac OS X. 
54 It is called Static OS X Server and can be downloaded from the main webpage. 
55 
 
56 Once downloaded it can be run in the same way as on any other Unix-like system. 
57 For more information please see the 'Running Murmur on Unix-like systems' above. 
58 
 
59 Running Murmur on Win32 
60 ======================= 
61 
 
62 Doubleclick the Murmur icon to start murmur. There will be a small icon on your 
63 taskbar from which you can view the log. 
64 
 
65 To set the superuser password, run murmur with the parameters '-supw <password>'. 
66 
 
67 Bandwidth usage 
68 =============== 
69 
 
70 Mumble uses 15 - 144 kbits/s incoming and outgoing when transmitting speech.
71 The default setting in a bandwidth requires 55 kbit/s per stream.
72 This is partly dependent on the compression scheme chosen: when the default 40 Kbps is used, sent data remains about 40 Kbps while received data is around half that for one stream.
73 If there are 10 users in a channel, your incoming bandwidth requirement will be ( 10 * 144 kbit/s ).
74 For the outgoing bandwidth, the maximum requirement in your server will be ( 144 kbit/s * 9 users * 10 streams = 12960 kbit/s )
