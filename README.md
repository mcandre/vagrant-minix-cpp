# vagrant-minix-cpp: a Vagrant box for building C/C++ binaries for MINIX

# DISCLAIMER

Syncing C/C++ artifacts back to the host directory is silently broken for some reason.

# ABOUT

vagrant-minix-cpp is a placeholder for a Vagrant box having a C/C++ compiler. In fact, MINIX (at least minix_R3.4.0rc6) includes `clang` by default, so users may wish to leverage the [mcandre/minix](https://app.vagrantup.com/mcandre/boxes/minix) base box instead.

# VAGRANT CLOUD

https://app.vagrantup.com/mcandre/boxes/vagrant-minix-cpp

# EXAMPLE

```console
$ vagrant up
$ vagrant ssh -c "cd /vagrant && clang++ -o hello hello.cpp && ./hello"
Hello World!
```

# RUNTIME REQUIREMENTS

* [Vagrant](https://www.vagrantup.com)
* The [VirtualBox](https://www.virtualbox.org) hypervisor provider

# BUILDTIME REQUIREMENTS

* [Vagrant](https://www.vagrantup.com)
* The [VirtualBox](https://www.virtualbox.org) hypervisor provider
* [make](https://www.gnu.org/software/make/)

# EXPORT

```console
$ make vagrant-minix-cpp.box
```
