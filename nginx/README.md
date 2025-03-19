## 1.18.0-zlib-ng.patch
* Patch created against Nginx 1.18.0
* Link to native zlib-ng instead of zlib
* Prefix all zlib calls
* Increase the size of pre-allocated memory to fit with zlib-ng requirements

## 1.26.2-zlib-ng.patch
* Patch created against Nginx 1.26.2
* Supports zlib-ng 2.2.x
* Links to native zlib-ng instead of zlib
* Prefixes all zlib calls
* Increases the size of pre-allocated memory to fit with zlib-ng requirements
* New: No longer requires you to define NGX_ZLIB_NG to enable overrides

## 1.26.3-zlib-ng.patch
* Patch created against Nginx 1.26.3
* Supports zlib-ng 2.2.x
* Links to native zlib-ng instead of zlib
* Prefixes all zlib calls
* Increases the size of pre-allocated memory to fit with zlib-ng requirements

PS: due to an oversight in the Nginx code, it assumes zlib is not compiled with
const support enabled, but zlib-ng always uses const.
So to avoid errors, please compile Nginx with this CFlag: `-Werror=discarded-qualifiers`
Ex: `./configure --with-cc-opt="-O2 -Werror=discarded-qualifiers"`
