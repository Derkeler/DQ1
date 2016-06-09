Title    : ClanRing CRMod++ v6.4 Quake Competition Server
Filename : crmod64.zip
Version  : 6.4
Date     : April 6, 2003
Author   : J.P. Grossman (a.k.a. Mephistopheles)
Email    : jpg@alum.mit.edu
URL      : http://planetquake.com/crmod

This is a Quake1 NETQUAKE mod.  It does not work with Quakeworld.  Do not send
us email asking us to make a Quakeworld version; we're not going to.

** LISTEN SERVER NOTE **  crmod 6.X will cause winquake listen servers to
lock up on Intel machines.  See section 15.4 of the manual for details.

** QSMACK NOTE **  crmod 6.X is not compatible with QSmack due to a problem
with qsmack message parsing.  If there is strong interest in fixing this,
an upgrade to qsmack might be made available.  However, there doesn't seem
to be much motivation for this now that crmod has full support for banning.


What's new?
=======================================

Not much, but a couple of important fixes:

- Fixed bug that allowed players to change colour during a match
- Restart an empty server after 6 hours to fix flashing glow bug
- Don't let players join a team during the last 5 seconds of a match countdown
  (unless the team needs more players)
- Put e2m6, e2m7, e3m7 and e4m8 back into the default levels.cfg
  (That file has been around for so long that I can't even remember why
  I didn't include those levels in the first place)
- added levelvoteon/levelvoteoff server console commands to enable/disable
  voting to change level


Description of crmod Files
=======================================
readme.txt       - This file
manual.txt       - Clanring CRMod++ v5.0 user's manual
autoexec.cfg     - Server startup config file
crmod.cfg        - Config file used to set the administrator password
levels.cfg       - Config file used to set the level order
userdefs.cfg     - Config file used to set the MOTD and custom levels
ban.cfg          - Config file used to store permanently banned ips
progs.dat        - Quake program data file run by the server
crmake.exe       - Utility to add the userdefs to progs.dat (Win32 build)
crmake.XXXXX     - Various operating system builds for the crmake utility
entities\*.ent   - Optional entity files
cameras\*.cam    - Optional camera files
config\*.cfg     - Optional config files (not included in crmod62.zip)

Description of other files
=======================================
qstrings.exe     - Utility for editing strings with the quake character set
dequake.exe      - Utility for converting quake characters to text characters
                   (win32 build)
dequake.linux    - Utility for converting quake characters to text characters
                   (linux build)

Dequake is useful for "decoding" name scripts or console logs so that they
can be viewed as text files.


Setup and Installation
=======================================
1. Create a subdirectory in your Quake directory called 'crmod' or whatever
   else you feel like calling it.
   
2. Unzip the contents of crmod64.zip into this new subdirectory.  Make sure that
   whatever program you use to unzip the files preserves the directory structure
   contained in crmod64.zip.

3. Edit autoexec.cfg, crmod.cfg, levels.cfg, ban.cfg and userdefs.cfg.  Each 
   of these files is commented with editing instructions.  Make sure you 
   change the passwords!  *Don't* give out password 0!!!

4. Run the crmake utility.  (crmake.exe in Win95/NT or crmake.linux in linux)

5. Start up your quake server with '-game crmod' in the command line replacing
   'crmod' with whatever name you gave your subdirectory.
   
Examples:  

  wqpro.exe -condebug -game crmod -dedicated +hostname godzilla 
  sqpro -condebug -game crmod -dedicated 16 +hostname bambi

The recommended quake executable for running a CRMod server is ProQuake
(http://planetquake.com/proquake).  It is also recommended that you use 
-condebug in the command line.  This will create a console log called
Qconsole.log in your crmod directory.  It is useful for seeing what has 
happened on your server, and it can also help the debugging process if you
encounter problems running crmod.  This file can also be given a different
name, or even named sequentially so that successive runs of the quake
executable don't overwrite previous log files (see the ProQuake manual
for details).

6. READ THE MANUAL!!!

Copyright
=======================================
All files included with this modification are Copyright 2000,
Idle Communications, Inc.

Author Information
=======================================
J.P. Grossman is a sixth year graduate student at M.I.T. in the department 
of Electrical Engineering and Computer Science.  He has been hacking Quake 
since Oct. '97 when he began working on the Elohim Server.  J.P. has been 
hacking computers in general for 23 years.  He started in grade 1 writing 
BASIC programs for a VIC-20 and saving them on a tape drive, often 
accidentally erasing the end of the previous program.

Acknowledgements
=======================================
Thanks to Paul Baker, author of Clanring 3.0-3.1 and co-author of 
CRMod++ 4.0-4.2.  Paul innovated such features as tournament mode for 
chasecams.  Thanks to Brian "Cool Cat" Whitlatch and Tom "Glocksmith" 
Greer Jr. for their assistance in testing the new compiler technologies 
that have been incorporated into crmod.

We would like to thank Ignatu (a.k.a. Frank Cabanski), who introduced Paul 
and J.P. to one another, for his patience and support throughout the early
stages of 4.0.  WE LOVE YOU FRANKY!  It would not have been possible to
create this server without the help of Tovi "Izra'il" Grossman, whose
suggestions, encouragement and bug reports, starting from the day the Elohim
Server was conceived, were invaluable.  Version 5.0 benefitted enormously
from the suggestions and bug reports of Mark "Turmoil" Santaniello and
Chris "Molotov" Ruvolo.  Thanks to Chris "ocor0ner" Van Wie from taking so
much pleasuer in making crmod crash - I owe you a drink.  Thanks also to 
Justin Hays and Dan "Nesta" at apci for their suggestions and their help 
with beta testing the Elohim Server versions 2.0 and up.  A big thanks
goes to Lance Vavricka for putting crmod 5.0 and up through its paces on his
linux box.  In particular, crmod 6.0 would crash and burn on linux if not
for his help.

Finally, thanks to everyone who has ever mailed in a suggestion or bug report;
this mod's for you!

License Agreement
=======================================
This modification is free for public and private non-commercial
use.  To use this modification for commercial purposes or to promote
any commercial venture, you must contact J.P. Grossman.

No modifications can be made to this mod with the exception
of the necessary config files as specified in this readme.

The ClanRing CRMod++ v6.3 Competition Server may be used on any server
without prior written permission provided that:

1. No persons shall be charged to play on any server running the mod.
2. It is not modified in any way except as stated in the
   installation section of this readme file.
3. It is not used in any way to promote commercial entities or ventures.
4. No llamas are harmed during the use of the server.

You may not distribute any of the files included with this modification!

If you would like to license the source code to this mod, please
contact jpg@alum.mit.edu

Technical Support
=======================================
Send all questions/bug reports/comments/suggestions to jpg@ai.mit.edu

Legal Notice
=======================================
The contents of this file and may change at any time, so don't blink. As with
all other mods, this software is provided "as is".  We are not responsible
for any personal losses or damages caused by this software which include, but
are not limited to, lack of sleep, reduced sex drive, nausea and vomiting,
loss of sight, serious bodily harm, financial destitution, termination of
relationships, death of pets or family members or self, loss of friends,
repetitive strain injury, lowered intelligence, and the complete erasure of 
all hard drive contents.  Of course, you can't wipe a hard drive with 
QuakeC.

Or can you? ;)

