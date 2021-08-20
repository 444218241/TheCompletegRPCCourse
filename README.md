# The Complete gRPC Course
> The Complete gRPC Course练习

## gRPC 完全教程 【Golang、Java】(中文字幕)
- `https://www.bilibili.com/video/BV1Rg411T7yF`
- `https://www.youtube.com/watch?v=2Sm_O75I7H0`

## Why is gRPC


## What is gRPC
- gRPC is a high-performance open-source feature-rich RPC framework.
- gRPC is originally developed by Google.
- Now it is a part of the Clod Native Computing Foundation(CNCF).
- g : stands for different things in each gRPC release: gRPC, green, good...
- RPC: Remote Procedure(正常)程序 Calls

## How gRPC works?

## Why gRPC users Protocol Buffer?
- Human-readable Interface Definition Language.
- Programming languages interoperable:
  - Code generators for many languages.
- Binary data representation:
  - Smaller size.
  - Faster to transport.
  - More efficient to serialize / deserialize.
- Strongly typed contract for safety.
- Conventions for API evolution.
  - Backward & forward compatibility.
- Alternative options:
  - Google flatbuffers.
  - Microsoft bond.

## What make gRPC efficient?
> gRPC uses http/2 as its transfer protocol.
- Binary framing
  - More performant and robust.
  - Lighter to transport , safer to decode.
  - Great combination with Protocol Buffer.
- Header compression using HPACK
  - Reduce overhead and improve performance.
- Multiplexing
  - Send multiple requests and responses in parallel over a single TCP connection.
  - Reduce latency and improve network utilization.
- Server push
  - One client request, multiple responses.
  - Reduce round-trip latency.

## HTTP/2 vs HTTP/1

|-|HTTP/2|HTTP/1|
|---|---|---|
|Transfer protocol|Binary|Text|
|Headers|Compressed|Plain text|
|Multiplexing|Yes|No|
|Requests Per Connections|Multiple|only once|
|Server Push |Yes|No|
|Release Year |2015|1997|

