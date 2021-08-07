---
layout: post
title: "My blog post"
date: 2021-05-22
---
Here is an interesting problem that I enjoyed solving.

# Problem statement

In a town, there are n people labeled from 1 to n. There is a rumor that one of these people is secretly the town judge.

If the town judge exists, then:

- The town judge trusts nobody.
- Everybody (except for the town judge) trusts the town judge.

There is exactly one person that satisfies properties 1 and 2.

You are given an array trust where trust[i] = [ai, bi] representing that the person labeled ai trusts the person labeled bi.

Return the label of the town judge if the town judge exists and can be identified, or return -1 otherwise.

For Example:
- For n = 2 and trust = [[1,2]] return 2, because 1 trusts 2, 2 trusts no one

# Understand 

### Happy cases:

Input: n = 3, trust = [[1,2],[3,2]]
Output: 2

Input: n = 4, trust = [[1,3],[1,4],[2,3],[2,4],[4,3]]
Output: 3

Input: n = 4, trust = [[1,2],[2,4],[3,4],[1,4]]
Output: 4

Input: n = 3, trust = [[1,2],[2,3]]
Output: -1

Input: n = 3, trust = [[1,3],[2,3],[3,1]]
Output: -1

Input: n = 2, trust = [[1,2],[2,1]]
Output: -1

