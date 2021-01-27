compose-etcd
============

Prerequisites
-------------

A MacOS installed Docker requires the following

Update hosts file with:

    172.16.238.11 etcd-0
    172.16.238.12 etcd-1
    172.16.238.13 etcd-2

Usage
-----

Start the cluster:

    $ docker-compose up -d

Stop the cluster:

    $ docker-compose down

Verify the cluster's health:

    $ source .env
    $ etcdctl --endpoints ${ENDPOINTS} cluster-health

License
-------

MIT
