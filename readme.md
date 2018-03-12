Freifunk TLDs for unbound
=========================

Ansible role to extract meta data from
[Freifunk Community Metadata](https://github.com/freifunk/icvpn-meta)
and configure stub zones for `unbound` to resolve these proprietary TLDs.


Variables
---------

* `ff_stub_zones_dir` (default `'ff_stub_zones'`):
  Directory where to place the stub files on the server.
  This is a immediate subdirectory of `/etc/unbound/`.

* `ff_community_data_dir` (default `'files/ff_communities'`):
  Directory where to find the Freifunk Community Metadata.

**Note:** Remove non-config files (like `README.md`) from the Freifunk Community Metadata
          as this role will not validate the file and data and fail.

References
----------

* [Freifunk Community Metadata](https://github.com/freifunk/icvpn-meta)
