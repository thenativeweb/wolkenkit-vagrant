# wolkenkit-vagrant

wolkenkit-vagrant provides a Vagrantfile to setup wolkenkit VMs.

## Installation

To run a wolkenkit VM, you need to [install Vagrant](https://www.vagrantup.com/downloads.html), version 2.0.4 or above.

If you use VirtualBox as virtualization engine, please make sure to also install the `vagrant-vbguest` plugin. This ensures that the guest additions in the VM will match your version of VirtualBox:

```shell
$ vagrant plugin install vagrant-vbguest
```

## Quick start

To run a wolkenkit VM, use the following command:

```shell
$ vagrant up
```

To stop the VM, run:

```shell
$ vagrant halt
```

If you don't need the VM any more and would like to delete it, use:

```shell
$ vagrant destroy
```

## License

The MIT License (MIT)
Copyright (c) 2018 the native web.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
