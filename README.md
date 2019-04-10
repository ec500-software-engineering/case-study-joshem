# case-study-joshem

## Technology & Platform

### Coding Language(s)
The coding languages used to implement Ethereum are actually quite varied. They have various different implementations within their framework.  You can use either a Go, C++, Java and Python based Ethereum implementation, all are offered from the team's Github account. All of these are official implementations, and are implemented independantly of one another. The repositories for each claim that they provide the Ethereum client as specified by the white paper. I will discuss and look at mostly the Go and C++ versions.

### Build Systems & Frameworks

Due to the different implementations, there are different build systems that are used for each implementation. For Go, it is required to use geth, the implementations Ethereum CLI. Building Geth requires a version of Go as well as a C compiler (I used gcc). It also requires the use of make to build. Once geth is built, you are able to use the Etheruem console through geth. 

The C++ version, referred to as aleth, uses Cmake in order to build it. It is noted on the readme for this that Visual Studio is in fact required for the Windows version. No build requirements were noted nor encountered for the *nix version.


### Testing 

The testing implementation for the Go repo is actually quite extensive. Tbey have several tests that are testing various different modules, including vm_utils, vm, state and many more. Furthermore, the testing framework is logged very extensively in a testdata directory. The tests here are further ordered into other directories, each of which contain a jsons which contain the expected output from the tests. There is a readme made foor the testing environment. In fact the testing environment is its own repo, with its own CI implementation. For the testing repo they are using Travis, while for the geth repo, they are using appveyor as well as Travis. The appveyor seems to work for Windows, while the travis platform is used for Linux and MacOS.
