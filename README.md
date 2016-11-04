# Bosh release for Apache Zookeeper

This is a Bosh release for Apache Zookeeper. This bosh release builds on the [Insightfactory Bosh release][1] in order to provide a standalone release for Apache Zookeeper.


## Supported Version

Apache Zookeeper 3.4.6

## Usage

Take a look at the manifests directory for sample deployment manifests. Edit required variables with erb tags.

To build:

1. Run `git clone https://github.com/samdai/max-zookeeper-boshrelease`
2. `cd zookeeper-boshrelease`
3. Run `bosh create release --force`
4. Run `bosh upload release`
5. Run `templates/make_manifest warden`
6. Run `bosh -n deploy`.
7. Run `bosh vms` to list VMs and IPs.


## TODO
*JDK 8 Testing

## Disclaimer

This is a development release and a work in progress. Please log issues. This release has been tested against AWS EC2

## Copyright and Credits

&copy; 2014, Murali Raju <murali.raju@appliv.com> [@murraju][3]


[1]: https://github.com/murraju/insightfactory-boshrelease
[3]: http://twitter.com/murraju
