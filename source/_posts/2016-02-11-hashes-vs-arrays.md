---
layout: post
title: "The quick, brown fox jumps over a lazy dog"
date: 2015-11-12 16:42:24
comments: true
description: "The quick, brown fox jumps over a lazy dog"
keywords: ""
categories:
- welcome
tags:
- welcome
---

When should you use a hash in place of an array (and vice versa)?  What even are hashes and arrays in the first place?  Hint: hashes are not at all related to hash browns.

Ok, let’s start with how they are similar.  Both are data structures!  This means that they can be used to store and look up data.  They can both hold many different types of objects (so they aren’t just limited to strings or integers).  The main difference is in how indexing is done; arrays use integer indexes, while hashes use arbitrary keys.
	
An array is essentially an ordered list.  Objects in arrays are assigned a numerical index.  Interestingly, the first term in an array is dubbed “0” and not “1” in most programming languages.  In the method array[x], you are looking for the element located x-elements away from the first element.  The first element is 0 units away from itself, so indexing starts at 0.  You can also use negative indexes to refer to how far away from the last unit in the array.  For example, in the array colors = [“blue”, “yellow”, “red”], colors[-2] refers to yellow.  While it’s nice that arrays are ordered, it’s hard to add things.  If you add something at the beginning, you have to push everything else a spot down.
	
A hash is a collection of key-value pairs.  Maybe I spoke too soon…It seems as if we could use hash browns in a hash function.  If we wanted to create a hash in ruby, we can use breakfast = { “beverage” => “orange juice”, “main” => “french toast”, “side” => “hash browns” }  Here, the first term is known as the key.  Because terms are identified by keys and not indexes, the keys must be unique.  That symbol => is notoriously known as the hash rocket, but there are more modern ways to create hashes that require less typing than the hash rocket, such as breakfast = {beverage: “orange juice”, main: “french toast”, side: “hash browns”}  Finally, the term after the hash rocket is known as the value. 

So, why would you use one instead of the other?  It really depends on the data.  If your data is ordered or if you might have duplicate values, then use an array.  If order doesn’t matter and all of your values must be unique, then use a hash.  Look-ups are usually faster in hashes as compared to arrays because they are based on arbitrary values instead of integers—instead of searching through every element of an array, the hash function can be used to quickly find the value once you have the key.

Resource 1: http://ruby-doc.org/core-2.2.0/Hash.html 
Resource 2: http://developeronline.blogspot.com/2008/04/why-array-index-should-start-from-0.html 
Resource 3: http://ruby-doc.org/core-2.2.0/Array.html 
Resource 4: http://stackoverflow.com/questions/6097637/whats-the-difference-between-arrays-and-hashes 
Resource 5: https://www.codecademy.com/forum_questions/52a69117282ae3085d000d63
Resource 6: http://stackoverflow.com/questions/25313658/when-is-it-better-to-use-an-array-instead-of-a-hash-in-perl  
