# 3-way integration test

This branch describes the [Bluechi](https://github.com/eclipse-bluechi/bluechi) - [Pullpiri](https://github.com/eclipse-pullpiri) - [Symphony](https://github.com/eclipse-symphony/symphony) integration testing process. The content is continuously updated.

**Note** : Pullpiri is currently under preparation. This document was written based on the former name, Piccolo.

## Test environment

Use 2 nodes with similar specification.

OS : CentOS Stream 9  
Architecture : x86-64

Disable firewalld  
selinux permissive mode

## Tool

### Bluechi

Refer to [Bluechi Documentation](https://bluechi.readthedocs.io/en/stable/getting_started/multi_node/).

### Piccolo

Clone [piccolo-bluechi](https://github.com/youngtaekiim/piccolo-bluechi). (temporary personal repository for testing.)  
Piccolo is built and runs at the container level, so there is nothing to install separately.

### Symphony

Clone [symphony-piccolo](https://github.com/youngtaekiim/symphony-piccolo).  
Since the symphony for piccolo has not been released yet, I have temporarily uploaded it to my personal repository.

I had to install the Golang build environment because my tests showed that it doesn't work well in containers, so I used a locally built binary. Refer to [install golang](https://go.dev/doc/install).