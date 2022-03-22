# Prebuilt binaries gRPC C++ for Windows
##### Current stable build of gRPC v1.44.0
##### gRPC [v1.44.0](https://github.com/grpc/grpc/releases/tag/v1.44.0) 

> They can be downloaded separately as zip archives from the  [releases](https://github.com/thommyho/gRPC_windows/releases) page


##### Releases

| Version | Commit | Debug | Release  | RelWithDebInfo | MSVC142 32Bit | MSVC142 64Bit | MSVC141 32 Bit | MSVC141 64 Bit | MSVC140 32 Bit | MSVC140 64 Bit | Example |
|---------|------------|-------|----------|----------------|---------------|---------------|----------------|----------------|----------------|----------------|---------|
| [1.44.0 ](https://github.com/thommyho/gRPC_windows/releases/tag/v1.44.0) | 591d56e1300b6d11948e1b821efac785a295989c  | :ballot_box_with_check: | :ballot_box_with_check: | :ballot_box_with_check:              | :ballot_box_with_check:             | :ballot_box_with_check:             | :ballot_box_with_check:              | :ballot_box_with_check:              | :ballot_box_with_check:              | :ballot_box_with_check:              | :ballot_box_with_check:       |

Build instructions from here: https://github.com/grpc/grpc/blob/master/BUILDING.md

Examples included. Tested with VS2015, VS2017 and VS2019 Enterprise and msvc140, msvc141, msvc142 (Win 10, SDK 10.0.19042)

#### Information about Build system and Tools

| Operating System | SDK Version   |
|------------------|---------------|
| Windows 10 (x64) |  10.0.19042   |

| Build Tool       | Version        |
|------------------|----------------|
| nasm             | 2.14.02        |
| cmake            | 3.19.2         |
| golang           | 1.17           |
| MSVC 140         | 19.0.24245.0   |
| MSVC 141         | 19.16.27045.0  |
| MSVC 142         | 19.29.30133.0  |

#### gRPC c++ Third Party Components

| Third Party Component | Version        | Commit                                   | Link                                                       |
|-----------------------|----------------|------------------------------------------|------------------------------------------------------------|
| abseil-cpp            | 20211102.0     | 215105818dfde3174fe799600bb0f3cae233d0bf | https://github.com/abseil/abseil-cpp                       |
| benchmark             |                | 0baacde3618ca617da95375e0af13ce1baadea47 | https://github.com/google/benchmark                        |
| bloaty                |                | 60209eb1ccc34d5deefb002d1b7f37545204f7f2 | https://github.com/google/bloaty                           |
| boringssl-with-bazel  |                | b9232f9e27e5668bc0414879dcdedb2a59ea75f2 | https://github.com/google/boringssl                        |
| cares                 |                | 6654436a307a5a686b008c1d4c93b0085da6e6d8 | https://github.com/c-ares/c-ares                           |
| envoy-api             |                | ff47e0a4bd03c0580305f9b138cc7937b63f7900 | https://github.com/envoyproxy/data-plane-api               |
| googleapis            |                | 2f9af297c84c55c8b871ba4495e01ade42476c92 | https://github.com/googleapis/googleapis                   |
| googletest            |                | 0e402173c97aea7a00749e825b194bfede4f2e45 | https://github.com/google/googletest                       |
| libuv                 | v1.37.0        | 02a9e1be252b623ee032a3137c0b0c94afbe6809 | https://github.com/libuv/libuv                             |
| opencensus-proto      | v0.3.0         | 4aa53e15cbf1a47bc9087e6cfdca214c1eea4e89 | https://github.com/census-instrumentation/opencensus-proto |
| opentelemetry         |                | 60fa8754d890b5c55949a8c68dcfd7ab5c2395df | https://github.com/open-telemetry/opentelemetry-proto      |
| protobuf              | v3.19.4        | 22d0e265de7d2b3d2e9a00d071313502e7d4cccf | https://github.com/google/protobuf                         | 
| protoc-gen-validate   |                | 9da36e59fef2267fc2b1849a05159e3ecdf24f3  | https://github.com/envoyproxy/protoc-gen-validate          |
| re2                   | 2021-09-01     | 8e08f47b11b413302749c0d8b17a1c94777495d5 | https://github.com/google/re2                              |
| xds                   |                | cb28da3451f158a947dfc45090fe92b07b243bc1 | https://github.com/cncf/xds                                |
| zlib                  | v1.2.11        | cacf7f1d4e3d44d871b605da3b647f07d718623f | https://github.com/madler/zlib                             |

#### Directory Setup for using/testing the provided HelloWorld-Example(s)

```console
.
+-- vs2015
|   +-- 0_HelperScripts
|   +-- 1_HelloWorld_Client
|   +-- 1_HelloWorld_Server
|   +-- 2_HelloWorld_Client_Callback
|   +-- 2_HelloWorld_Server_Callback
|   +-- 3_HelloWorld_Client_Async_1
|   +-- 3_HelloWorld_Client_Async_2
|   +-- 3_HelloWorld_Server_Async
|   +-- 4_HelloWorld_Client_Compression
|   +-- 4_HelloWorld_Server_Compression
|   +-- 5_HelloWorld_Client_Load_Balancing
|   +-- 5_HelloWorld_Server_Load_Balancing
|   +-- 6_HelloWorld_Client_Meta
|   +-- 6_HelloWorld_Server_Meta
|   +-- 7_KeyValueStore_Client
|   +-- 7_KeyValueStore_Server
|   +-- 8_Route_Guide_Client
|   +-- 8_Route_Guide_Server
|   +-- 9_Route_Guide_Client_Callback
|   +-- 9_Route_Guide_Server_Callback
|   +-- protos
|   +-- res
|   +-- Examples_vs2015.sln
+-- vs2017
|   +-- 0_HelperScripts
|   +-- 1_HelloWorld_Client
|   +-- 1_HelloWorld_Server
|   +-- 2_HelloWorld_Client_Callback
|   +-- 2_HelloWorld_Server_Callback
|   +-- 3_HelloWorld_Client_Async_1
|   +-- 3_HelloWorld_Client_Async_2
|   +-- 3_HelloWorld_Server_Async
|   +-- 4_HelloWorld_Client_Compression
|   +-- 4_HelloWorld_Server_Compression
|   +-- 5_HelloWorld_Client_Load_Balancing
|   +-- 5_HelloWorld_Server_Load_Balancing
|   +-- 6_HelloWorld_Client_Meta
|   +-- 6_HelloWorld_Server_Meta
|   +-- 7_KeyValueStore_Client
|   +-- 7_KeyValueStore_Server
|   +-- 8_Route_Guide_Client
|   +-- 8_Route_Guide_Server
|   +-- 9_Route_Guide_Client_Callback
|   +-- 9_Route_Guide_Server_Callback
|   +-- protos
|   +-- res
|   +-- Examples_vs2017.sln
+-- vs2019
|   +-- 0_HelperScripts
|   +-- 1_HelloWorld_Client
|   +-- 1_HelloWorld_Server
|   +-- 2_HelloWorld_Client_Callback
|   +-- 2_HelloWorld_Server_Callback
|   +-- 3_HelloWorld_Client_Async_1
|   +-- 3_HelloWorld_Client_Async_2
|   +-- 3_HelloWorld_Server_Async
|   +-- 4_HelloWorld_Client_Compression
|   +-- 4_HelloWorld_Server_Compression
|   +-- 5_HelloWorld_Client_Load_Balancing
|   +-- 5_HelloWorld_Server_Load_Balancing
|   +-- 6_HelloWorld_Client_Meta
|   +-- 6_HelloWorld_Server_Meta
|   +-- 7_KeyValueStore_Client
|   +-- 7_KeyValueStore_Server
|   +-- 8_Route_Guide_Client
|   +-- 8_Route_Guide_Server
|   +-- 9_Route_Guide_Client_Callback
|   +-- 9_Route_Guide_Server_Callback
|   +-- protos
|   +-- res
|   +-- Examples_vs2019.sln
# Extract the prebuilt bins and libs like this for your disired toolchain e.g.:
+-- MSVC142_64
|   +-- Debug
|       +-- bin
|       +-- cmake
|       +-- include
|       +-- lib
|       +-- share
|   +-- Release
|       +-- bin
|       +-- cmake
|       +-- include
|       +-- lib
|       +-- share
|   +-- RelWithDebInfo
|       +-- bin
|       +-- cmake
|       +-- include
|       +-- lib
|       +-- share
+-- MSVC142_32 ...
+-- MSVC141_64 ...
+-- MSVC141_32 ...
+-- MSVC140_64 ...
+-- MSVC140_32 ...
```
