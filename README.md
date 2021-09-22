# About Perl Chat:
There are two goals I set forth when I began Perl Chat. The first of these two goals was to learn Perl sockets, as well as to get a better feeling for Perl in general. The second of these was to write some software that could be useful to someone some day somewhere.

The idea of a chat server/client is not new. There are dozens of them already out there. However, none of them were written in Perl, and none of them were designed to run independently of other communications services. I found there were many other clones out there of IM software, but none that suited my needs. So I decided that this would be an opportune time for me to learn Perl, and to write something I wanted.

This software was designed to be used on a small scale, in a relativly trusted environment. For example, a private LAN found on a University, in an apartment complex, or at work.

# Installation:
First of all you need a working version of Perl. Preferably 5.6 but 5.005X should also work fine. For versions of Perl Chat < 0.1.0 you will need to compile Perl with Threads. (Keep in mind that Threads are still experimental) I designed this program with Perl 5.6.0 which can be found HERE.
You will need to read the installation instructions to compile it with Threads. I advise anyone who is doing this to install this new version of perl into /usr/local/ so as to not overwrite your old perl. Then by changing the first line of the script you can toggle between the different installs of perl.

You will also need module:
Tk800.022: which can be found http://www.cpan.org/authors/id/N/NI/NI-S/Tk800.022.tar.gz

You have to uncompress this module ('tar -zxvf file.tar.gz'), and then compile it ('/usr/local/bin/perl Makefile.PL' followed by 'make', followed by 'make test', followed by 'make install'). Refer to the README's in the various archives for more detailed information.

If you are in windows you can get Active Perl from Active State and then use the Perl Package Manager (ppm for short) to install the modules. There is more info at the Active State web site.

Though it has not been tested yet this should run under Windows 2000. Download Active Perl 5.6 from Activestate
When that is done go into console mode and type 'ppm', this stands for Perl Package Manager. Then type 'install Tk', this will install the Tk module needed for the GUI. That is all, you should be able to run Perl Chat server and client from the console or from double clicking on the sourcefiles. Update: I have been fooling around with this for a while now and I cannot get the threads to work with any precompiled binary versions of Active Perl. I imagine you will have to compile perl yourself and enable threads. If anyone knows of a link to a binary version of Perl for win32 with Threads enabled please email me.

# Trouble Shooting:
Make sure the first line of client.pl and server.pl is the path to your Perl Interpreter.
Make sure the Tk module is installed.
Under Win32 Im getting a strange error message when I run either the client or the server... Im working on it...
Currently there is no check on where the perlchat.gif file is, so if the program crashes while you are trying to view About->About, make sure the gif is in the same directory as the program.

# License:
I have placed Perl Chat under the GNU General Public License.

# Credits:
As always thanks go out to all of the other developers that made my work environment possible. This includes all the Perl hackers who created and debugged Perl, all the Kernel hackers who made Linux the gem that it is, and all of the people who have helped me on irc.dal.net in #perl.

Project also hosted at http://perlchat.sourceforge.net/
