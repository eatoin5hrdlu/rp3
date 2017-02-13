# rp3
Buildroot handoff Raspberry Pi 3




What I'd like in an off-the-shelf Raspberry Pi.

I spend close to a whole day, turning a new Raspberry Pi 3 into a usable machine.  Among the things I'd like in a buildroot image are:


Remote log in capability:
Requires: 
   1) tightvncserver : xrdp now seems broken (microsoft)
   2) The following command added to /etc/rc.local)

/usr/bin/x11vnc -xkb -auth /var/run/lightdm/root/:0 -noxrecord -noxfixes -noxdamage -rfbauth /etc/x11vnc.pass -forever -bg -rfbport 5900 -o /var/log/x11vnc.log  > /dev/null 2>&1

   3) Edit smstext.py (change phone number) and add to /etc/rc.local
     (It sends a text message with the current IP addresses).

Allowing remote login to a brand-new raspberry pi without a keyboard or mouse.

OTHER PACKAGES:

	mg         (really tiny Emacs-like editor)
	build-essential
	alsa-utils
	openCV
	supercollider
	swi-prolog



