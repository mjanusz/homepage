*INFORMATION*: I'm looking for a new maintainer for this project. Maintaining
fbcondecor usually requires little effort, and only infrequent changes to the
code to match updates made in the kernel framebuffer layer. That being said,
there are still new features that could be implemented (e.g. adding support for
console rotation) if you have the inclination to do so. Fbcondecor can be a
nice project to get familiar with the framebuffer console code in the kernel.
Please drop me an e-mail if you're interested. I can provide a quick overview
of the code to get you up to speed quickly and suggest things to be done.

Overview
--------
fbcondecor stands for Framebuffer Console Decorations. It is a kernel patch
that adds eye-candy by making it possible to display pictures in the background
of system consoles. In order for the patch to work properly, a userspace helper
application called fbcondecor_helper has to be installed. This application is
currently provided as a part of fbsplash.

History
-------
At first, the features of both fbsplash and fbcondecor were provided by a
single kernel patch called bootsplash (developed by Stefan Reinauer, Kenneth
Wesley Wimer II, Michael Schroeder and Volker Poplawski). It was a solution
which mostly worked just fine, but had a number of problems and limitations
(JPEG decoder in the kernel, etc). In 2004, the gensplash project was created
(by the author of this text, Michal Januszewski). It aimed at creating a
sanitized version of bootsplash and moving as much code as possible to
userspace.

As parts of this project, fbsplash and splashutils were developed. fbplash was
a kernel patch that made it possible to display background pictures on the
system consoles, and splashutils were a collection of programs for controlling
fbsplash and for displaying the "silent" splash screen (image with a progress
bar, icons, etc).

This naming scheme was problematic in two ways. First, fbsplash didn't actually
have anything to do with the silent splash screen, as its name could have
suggested. Second, many people were confused as to what was necessary to get
the silent splash working and didn't realize they only needed the userspace
part (splashutils) for this.

Thus, in August 2007, in the hope of making things more clear and easy to
understand, the fbsplash patch was renamed to fbcondecor and the gensplash
project took the name of fbsplash.

Troubleshooting
---------------
* I patched my kernel with fbcondecor and I can't see any new options in the
  configuration menu.

Please make sure that you have the "Framebuffer Console support"
(FRAMEBUFFER_CONSOLE) option enabled and the "Enable Tile Blitting Support"
(FB_TILEBLITTING) option disabled.
