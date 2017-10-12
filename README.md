Role Name
=========

Ansible Role for installing Go binaries or building Go locally.

Requirements
------------

A machine with minimum 1024 MB RAM

Role Variables
--------------

BUILD_FROM_SRC: false                   # Whether to build Go from source (if true) or install binary (if false)
GODEST: /usr/local                      # Directory for installing Go and Go related files
GOROOT: $GODEST/go                      # Installation location for Go
GOPATH: $GOROOT/bin                     # Go Executable location
GOVER: 1.9.1                            # Version of Go to install / build
GOVER_CHECKSUM: "sha256:xxxx"           # Checksum for the Go version to be downloaded (if installing binary file)

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

``` yaml
- hosts: all
  gather_facts: no

  roles:
    - { role: mohitsharma44.gorole }

```

License
-------

MIT

Author Information
------------------

Mohit Sharma.
github.com/mohitsharma44
