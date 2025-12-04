---
layout: post
title: "Understanding Containerization with Docker: Key Concepts"
date: 2025-12-04 15:30:00 +0600
categories: [DevOps, Cloud]
tags: [docker, containerization, devops, learning]
---

## Docker: Why is it crucial in Modern Development?

কন্টেইনারাইজেশন (Containerization) হলো অ্যাপ্লিকেশনকে তার সকল ডিপেন্ডেন্সি এবং কনফিগারেশন সহ একটি কন্টেইনারে প্যাকেজ করার প্রক্রিয়া। আমি বর্তমানে এটি শিখছি এবং এটি ডেভেলপারদের জন্য খুবই গুরুত্বপূর্ণ। 

### ১. ইম্যুটেবল ইনফ্রাস্ট্রাকচার (Immutable Infrastructure)

এর মানে হলো একবার কন্টেইনার তৈরি হয়ে গেলে, এটি আর পরিবর্তন করা যায় না। কোনো আপডেটের দরকার হলে, একটি নতুন কন্টেইনার তৈরি করে রিপ্লেস করা হয়।

### ২. পরিবেশের সমতা (Environment Consistency)

Docker ব্যবহার করে, "It works on my machine" সমস্যা দূর হয়। ডেভেলপমেন্ট, টেস্টিং এবং প্রোডাকশন এনভায়রনমেন্টে কোড একই কন্টেইনারের মধ্যে রান করে, যা পরিবেশের সমতা নিশ্চিত করে।

### ৩. মূল ডকার কমান্ডস (Essential Docker Commands)

* `docker build . -t my-app`: ডকারফাইল ব্যবহার করে ইমেজ তৈরি করা।
* `docker run -d -p 8080:80 my-app`: ইমেজ থেকে কন্টেইনার রান করা এবং পোর্ট ম্যাপ করা।
* `docker exec -it <container-id> /bin/bash`: চলমান কন্টেইনারের ভেতরে প্রবেশ করা।