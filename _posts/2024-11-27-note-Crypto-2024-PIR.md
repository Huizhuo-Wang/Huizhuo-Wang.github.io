---
layout: post
title: PIR 研究进展
date: 2024-11-20
Author: Huizhuo Wang
tags: [note, Private Information Retrieval]
comments: true
toc: true
pinned: true
---

此文章主要介绍 2024 年隐私信息检索（Private Information Retrieval, PIR）在三大密码学会议上的的研究进展。

## [CRYPTO 2024] Fully Malicious Authenticated PIR

### 研究背景

经过身份验证的 PIR 使服务器能够最初提交到包含 N 个项目的数据库，客户端稍后可以私下获取复杂度为 N 的次线性的单个项目，并保证检索到的项目与提交的数据库一致。一个关键要求是中止隐私，即服务器不应了解有关查询的任何信息，即使它知道客户端是否中止。Colombo 等人 (USENIX '23) 最近考虑了这个问题，他们提出了在数据库诚实提交的假设下安全的解决方案。在这里，我们弥补了他们基于 DDH 的方案的这一差距，并提出了一种解决方案，可以容忍提供潜在畸形承诺的完全恶意服务器。我们的方案具有通信和客户端计算复杂度 Oλ( √ N)，不需要任何额外的假设，并且不会引入繁重的机制（例如，通用简洁证明）。我们通过引入验证查询来实现这一点，从服务器的角度来看，这些查询在计算上与常规 PIR 查询没有区别。假设服务器成功正确回答 κ 个这样的验证查询，则客户端有 1 − 1 2κ 的概率确信服务器无法通过中止来破坏隐私。
