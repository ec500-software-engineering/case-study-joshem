# case-study-joshem

## Technology & Platform

### Coding Language(s)
The coding languages used to implement Ethereum are actually quite varied. They have various different implementations within their framework.  You can use either a Go, C++, Java and Python based Ethereum implementation, all are offered from the team's Github account. All of these are official implementations, and are implemented independantly of one another. The repositories for each claim that they provide the Ethereum client as specified by the white paper. I will discuss and look at mostly the Go and C++ versions.

### Build Systems & Frameworks

Due to the different implementations, there are different build systems that are used for each implementation. For Go, it is required to use geth, the implementations Ethereum CLI. Building Geth requires a version of Go as well as a C compiler (I used gcc). It also requires the use of make to build. Once geth is built, you are able to use the Etheruem console through geth. 

The C++ version, referred to as aleth, uses Cmake in order to build it. It is noted on the readme for this that Visual Studio is in fact required for the Windows version. No build requirements were noted nor encountered for the *nix version.
