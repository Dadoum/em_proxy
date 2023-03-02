# Emotional Mangling Proxy

What Apple and I both share after this is done

## What is EMP

A transparent interface level proxy for TCP packets. This project is designed to work around the loopback limitations on iOS.

## How does it work

By modifying packets and retransmitting them back through a WireGuard tunnel

## How to build

``cargo build --target aarch64-apple-ios``

## Publishing new release

We use a github action to generate a `.xcframework` for use in Swift PM or XCode.

This overwrites the last build on the tag `Build`.

Either push a commit with `[build]` as the prefix for the commit message or push an empty commit with:

```
git commit --allow-empty -m "[build]"
```

## ETA wen

June 2069
