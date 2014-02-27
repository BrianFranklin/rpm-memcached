rpm-memcached
=============

An RPM spec file build and install memcached 1.4.x with slab reassignment.

To Build:

`sudo yum -y install rpmdevtools && rpmdev-setuptree`

`sudo yum -y install libevent-devel`

`wget http://www.memcached.org/files/memcached-1.4.17.tar.gz -O ~/rpmbuild/SOURCES/memcached-1.4.17.tar.gz`

`wget https://raw.github.com/nmilford/rpm-memcached/master/memcached.spec -O ~/rpmbuild/SPECS/memcached.spec`

`rpmbuild -bb ~/rpmbuild/SPECS/memcached.spec`
