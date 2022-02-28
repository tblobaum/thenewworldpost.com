---
layout: post
author: HN
title: Writing an OS in Rust
slug: 2022-02-27-learn-rust-by-writing-a-small-os
date: '2022-02-27'
categories: HN
tags: ''
featured-image: ''
featured-image-alt: ''
---
This post adds support for heap allocation to our kernel. First, it gives an introduction to dynamic memory and shows how the borrow checker prevents common allocation errors. It then implements the basic allocation interface of Rust, creates a heap memory region, and sets up an allocator crate. At the end of this post all the allocation and collection types of the built-in `alloc` crate will be available to our kernel.

[_read more »_](https://os.phil-opp.com/heap-allocation/)
