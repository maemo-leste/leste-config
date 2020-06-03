leste-config
============

This repo contains specific Leste configurations, and builds them as
packages specific to our device targets.


HOWTO
-----

* https://debathena.mit.edu/config-package-dev/
* https://wiki.debian.org/ConfigPackages


tl;dr
-----

1. Create a new directory called `leste-config-$target`.
2. Append the new package to `debian/control` (just see what is already
   there)
3. Add files inside their respective directories and make sure they have
   a **.leste** suffix if you want them to be added to the system.
4. Once added, to go the `debian` directory and run `gen_displace` once.
   This will generate the `.displace` and `.install` files in place.
5. Update `debian/changelog`

**N.B.** All standard maintenance stuff applies. Use git, branches, and
tags.
