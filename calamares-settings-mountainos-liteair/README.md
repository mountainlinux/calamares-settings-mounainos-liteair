This package exists to house MountainOS settings for the Calamares installer.

If you want to add a new package for your flavor, here's how to do it:
 1. Create a new top-level directory (like MountainOS, you could just copy
    theirs and customize).
 2. Edit files and rename the branding directory for your flavor. All of the
    configuration files are pretty self-explanatory, but they're documented
    well upstream, so it shouldn't be hard to put your own spin on things.
 3. Create a new binary package, and *make sure to Conflicts against all other
    binary packages in this source package*. This needs to be done because all
    subdirectories are installed in the same location, so this makes sure that
    nobody tries to install any two binary packages at the same time.

That's about it. If you have any questions, feel free to email us
at mountainoslinux@gmail.com or consult the upstream documentation.
