<p><img src="https://avatars1.githubusercontent.com/u/12563465?s=200&v=4" alt="OCI logo" title="oci" align="left" height="70" /></p>
<p><img src="https://miro.medium.com/max/300/1*76dYSeZfdwypV1bzlwPivg.gif" alt="Lighthouse logo" title="lighthouse" align="right" height="80" /></p>

Container File ⛵ 🔗 Lighthouse
=========
![GitHub release (latest by date)](https://img.shields.io/github/v/release/0x0I/container-file-lighthouse?color=yellow)
[![0x0I](https://circleci.com/gh/0x0I/container-file-lighthouse.svg?style=svg)](https://circleci.com/gh/0x0I/container-file-lighthouse)
[![Docker Pulls](https://img.shields.io/docker/pulls/0labs/lighthouse?style=flat)](https://hub.docker.com/repository/docker/0labs/lighthouse)
[![License: MIT](https://img.shields.io/badge/License-MIT-blueviolet.svg)](https://opensource.org/licenses/MIT)

an Ethereum 2.0 client, written in Rust and maintained by Sigma Prime

**Overview**
  - [Setup](#setup)
    - [Build](#build)
    - [Config](#config)
  - [Operations](#operations)
  - [Examples](#examples)
  - [License](#license)
  - [Author Information](#author-information)

#### Setup
--------------
Guidelines on running service containers are available and organized according to the following software & machine provisioning stages:
* _build_
* _config_
* _operations_

##### Build

...*steps for building container images based on various use-cases/targets*...

###### targets

| Name  | description |
| ------------- | ------------- |
| `test`    | image containing service binaries, test tools and functional test cases for validation |
| `release` | minimal resultant image containing service binaries, entrypoints and helper scripts |

```bash
docker build --target <target> .
```

##### Config

...*description of service container instance configuration options*...

`$DEMO_USER` **default**: *world*

* username to say hello to when visiting the demo website!

###### port mappings

...*network ports service containers listen on for various functions and details involving operator customizations*...

| Port  | mapping description | type | config setting | command-line flag |
| ------------- | ------------- | ------------- | :-------------: | :-------------: |
| `80`    | Apache web server | *TCP*  | `-` | `-` |

#### Operations

...*guidelines for performing operational tasks on service container instances*...

Examples
----------------
default example:
```
docker run --env DEMO_USER=<user> 0labs/demo:<tag>
```

License
-------

MIT

Author Information
------------------

This Containerfile was created in 2021 by O1.IO.

🏆 **always happy to help & donations are always welcome** 💸

* **ETH (Ethereum):** 0x652eD9d222eeA1Ad843efec01E60C29bF2CF6E4c

* **BTC (Bitcoin):** 3E8gMxwEnfAAWbvjoPVqSz6DvPfwQ1q8Jn

* **ATOM (Cosmos):** cosmos19vmcf5t68w6ug45mrwjyauh4ey99u9htrgqv09
