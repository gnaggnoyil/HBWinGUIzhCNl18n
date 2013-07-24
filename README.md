For license issues, see the "license" file.

How to compile

v0.9.9

First you need to get the following tools ready:
  Visual Studio 2010 or 2012
  Unicode NSIS toolchain with inet plugin installed
    
Then patch the patch file to the HandBrake v0.9.9 svn snapshot(using '-p1'
paramater).

Go to HandBrake snapshot\win\CS\ directory, make a new directory called bin.
Then enter bin directory and make a new directory called Release. Copy Fonts
directory, HandBrakeCLI.exe and hb.dll that has been compiled previously
into Release directory.

Open Visual Studio Command Prompt, enter the HandBrake snapshot\win\CS\
directory, and run msbuild using build.xml, with a Release build targeting
x86 or x64.

Finally go to win\CS\HandBrakeWPF\bin\Release and grab the installer out,
which has a name like "HandBrake-0.9.9-Win_GUI-zh_CN.exe". That's what we
finally get.

Then you can simply run the installer and install this application on your
operating system.