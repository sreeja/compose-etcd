compose-etcd
============

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
