### About

This repository is here to allow sharing patches that allow compiling an application against zlib-ng.
The patches should generally be safe to use in prod.
The patches might not be implemented in a clean way, they might short-circuit zlib detection or otherwise
hard-code zlib-ng usage, therefore these patches might not be of a quality where they are ready to upstream.

### Contribution guidelines

* Look at the nginx patch folder for an example of how things should look.
* Add a folder for the application name, with a README.md file describing its contents.
* Add a short description to the README.md, detailing the changes per patch file.
* Optionally add a longer description to the top of the patch file.
* Add information about what version the patch applies cleanly to, preferably also as part of the patch name.

