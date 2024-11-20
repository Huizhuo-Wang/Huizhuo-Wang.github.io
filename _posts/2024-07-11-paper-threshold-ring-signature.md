---
layout: post
title: 学术论文 "Threshold ring signature - generic construction and logarithmic size instantiation"
date: 2024-07-11
Author: Huizhuo Wang
tags: [paper, ring signature]
comments: true
toc: true
pinned: true
---

> title: "Threshold ring signature: generic construction and logarithmic size instantiation"
> date: 2024-07-11
> venue: 'Cybersecurity'
> paperurl: [https://link.springer.com/article/10.1186/s42400-024-00233-9](https://link.springer.com/article/10.1186/s42400-024-00233-9)
> citation: Huizhuo Wang, Yang Tao and Rui Zhang. Threshold ring signature: generic construction and logarithmic size instantiation. Cybersecurity 7, 46 (2024). https://doi.org/10.1186/s42400-024-00233-9.

## Abstract

A ring signature is a variant of normal digital signature and protects the privacy of a specific signer in the sense that a ring signature can be verified, but the signer’s identity can only be traced to a limited set.
The concept was further enhanced to threshold setting to distribute signing ability among several signers.
Since threshold ring signature was introduced, it was a hard problem whether one can have efficient constructions for it.
In this paper, we introduce a new generic construction of threshold ring signature, named GTRS, based on canonical identification of a specific form.
Our signature consists of a polynomial (represented by $n-t+1$ coefficients) and a single response, resulting in significantly shorter threshold ring signatures.
Instantiating the generic construction with specific DL-based components, e.g. Schnorr identification and a novel vector argument of knowledge developed in this paper, we obtain GTRS-EC, which is shorter than all existing threshold ring signatures without any trusted setup.
