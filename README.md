# s2i-test-vm

A Vagrant VM for testing [s2i](https://github.com/openshift/source-to-image) builder images.
It executes a provisioning script, insalling:

* [git](https://git-scm.com)
* [Docker](http://docker.io)
* [go](http://golang.org)
* [s2i](https://github.com/openshift/source-to-image)

## Usage

```shell
vagrant up
vagrant ssh
```

Inside the VM, clone the builder image repository you want to test an then run your tests. Example:

```shell
git clone https://github.com/codecentric/springboot-maven3-centos.git
cd springboot-maven3-centos
sudo make test
``

## Copyright

Released under the Apache License 2.0. See the [LICENSE](https://github.com/codecentric/s2i-test-vm/blob/master/LICENSE) file.
