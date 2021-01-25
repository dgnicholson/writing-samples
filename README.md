# Writing Samples Overview

## API reference

This sample is an exercise to create reference documentation for a real API. I used Postman and curl to help create it. 

## Excel 2016 instructor guide

This document is part three of a four-part course that teaches Microsoft Excel 2016. It teaches more advanced features of Excel and is intended for instructors to use when administering lessons. A student version of this document is very similar but leaves out instructor only content. Note that this is a small sample of a larger document. 

## How to play tic-tac-toe

This sample is from an exercise to write a short document that describes how to play tic-tac-toe. The audience is an intelligent adult who has never heard of the game. 

## Native library API reference

This sample is from an exercise to write an API reference document that explains how to call the following method. 

```Java
public static void findNeedles(String haystack, String[] needles) {
if (needles.length > 5) {
  System.err.println("Too many words!");
  } else {
  int[] countArray = new int[needles.length];
    for (int i = 0; i < needles.length; i++) {
  String[] words = haystack.split("[ \"\'\t\n\b\f\r]", 0);    
    for (int j = 0; j < words.length; j++) {
  if (words[j].compareTo(needles[i]) == 0) {
    countArray[i]++;
      }
    }
  }
for (int j = 0; j < needles.length; j++) {
System.out.println(needles[j] + ": " + countArray[j]);
      }
    }
}
```
The audience is an experienced Java programmer.

## Quickstart diagram

This quickstart guide was created for a hardware product that enables PTT (push-to-talk) functionality on satellite phones. Its intended audience includes those who just purchased the product and want to set up the system and understand its basic functionality.  

## Technical product overview (blog post)

This content is for [a blog post on the company website](https://sigmastcomms.com/what-is-rcs/). The purpose of this post is to provide a quick conceptual overview of what RCS (Rich Communication Services) is and how it can impact users. It’s aimed at both technical and general audiences who are not familiar with RCS.
