# Memory Allocators

# Comparison Summary

| Allocator                                                  | Language | Maintainer / Organization                                             | License                        | Rust Binding                                                      |
|------------------------------------------------------------|----------|-----------------------------------------------------------------------|--------------------------------|-------------------------------------------------------------------|
| [jemalloc](https://github.com/jemalloc/jemalloc)           | C        | Originally Jason Evans, currently community & Meta-backed maintenance | BSD-2-Clause                   | [tikv-jemallocator](https://github.com/tikv/jemallocator)         |
| [mimalloc](https://github.com/microsoft/mimalloc)          | C        | Microsoft Research / Daan Leijen                                      | MIT                            | [mimalloc crate](https://github.com/purpleprotocol/mimalloc_rust) |
| [ptmalloc (glibc malloc)](https://sourceware.org/glibc/)   | C        | GNU Project                                                           | LGPL-2.1+                      | -                                                                 |
| [rpmalloc](https://github.com/mjansson/rpmalloc)           | C        | Mattias Jansson                                                       | Public Domain / Unlicense      | -                                                                 |
| [TCMalloc](https://github.com/google/tcmalloc)             | C++      | Google                                                                | Apache-2.0                     | -                                                                 |
| [snmalloc](https://github.com/microsoft/snmalloc)          | C++      | Microsoft Research & University of Cambridge Computer Laboratory      | MIT                            | [snmalloc-rs](https://github.com/microsoft/snmalloc)              |
| [Scudo](https://llvm.org/docs/ScudoHardenedAllocator.html) | C++      | LLVM Project                                                          | Apache-2.0 with LLVM Exception | -                                                                 |

