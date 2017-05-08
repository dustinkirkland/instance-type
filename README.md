## Synopsis

Each public cloud has its own named instance types, with specific resource allocation: at least CPU and Memory, and sometimes more (disk, GPU, pricing, and other attributes).

This project provides a freely available, well-maintained mapping of instance type names and at least the most common attributes, in several formats (tabular, yaml).

## Code Example

Import the tabular or yaml files into your project, when you need to translate from a cloud's magic word for an instance type, into its attributes.

## Motivation

This project exists in a common location so that a project like LXD, KVM, OpenStack, MAAS, or otherwise easily create containers, virtual machines, or physical machines that rougly map to equivalent instance sizes in Amazon, Azure, Google, or other public clouds.

For example, you can use LXD to easily create a new container instance whose performance profile matches an AWS m1.large (or any other Amazon instance type):

```
$ lxc launch --type m1.large ubuntu:16.04
```

## Contributors

Other cloud instance type contributions are welcome.  Please create a new tab-delimited file in the tab/ directory.  The first column is the instance type's name, the second column is the number of CPUs, and the third column is the memory allocation in GiB.

## License

Copyright 2017 @DustinKirkland

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License.  You may obtain a copy of the License at:

 * http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  See the License for the specific language governing permissions and limitations under the License.
