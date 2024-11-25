---
title: Spring 2023 Course Reviews
topics: ["review"]
date: 2023-05-04
---

## Overview

Considering I dropped 15-150 after the first lecture, I found this semester to be, on average, light/moderate. However, the courses I took weren’t great, relative to previous semesters. Despite that, this semester I took an interest in machine learning after taking 10-301.


### 18-349 Introduction to Embedded Systems

Taught by Nace and Rowe, this course was being reworked to be less software-intensive(?) than previous versions of the course, mainly due to the removal of Kernel Lab in favor of using FreeRTOS (whether this was a good decision is debatable). Breadth of topics was focused on a lot more than depth. In lectures, a lot of topics (maybe too many) in the embedded programming space were discussed, such as code optimization, internet of things, and task scheduling, to name a few. Overall, lecture content taught enough for students to be aware of certain concepts in the embedded world.

The graded assignments in this class were quizzes (to be completed in-class) and labs (to be completed outside of class). Quizzes for the first half of the class were pop quizzes, which almost everyone dreaded. The policy was changed mid-semester, so that the professors would have to announce it 24 hours before. Quizzes usually covered content from the previous two lectures. They weren’t difficult, but they require a lot of memorization (which I found to be annoying), and previous lectures can be up to about 60 slides in length.

Labs, minus the first lab and PCB lab, are Arduino-style programming assignments, where you code hardware drivers and implement some hardware mechanism, such as a lock or a temperature sensor, using software. The boards used in these labs are STM32s, specifically the Nucleo STM32F401s, which are ARM-based. If you end up taking this class, one thing you’ll notice is that a significant portion of the difficulty comes from trying to interpret the vague datasheets that come with these boards. A major gripe I have with this class is that most of the labs just devolve into writing hardware drivers with questionable software design choices and lack of regard for robustness. The hardest lab was probably writing a interrupt-based UART driver without race-conditions and without data garbling/loss. The main difficulty in writing this wasn’t the actual driver, but was making it fast and robust enough so that it could handle a high packet-rate. This would be tested with a python script that would send these packets to your board at a relatively high speed; however, this requirement was eventually turned into extra-credit due to how many people couldn’t get it working (possibly due to faulty UART implementations or the virtual machines sucking). Despite the dissatisfaction I had with many of the labs, I did learn some cool things such as manufacturing a PCB and implementing PID.

In summary, despite the amount of content that was covered in lecture, the corresponding labs were shallow and repetitive. I wish the labs were more creative and high-level (using driver libraries instead of having to code it manually each time). An idea related to IoT would maybe be having the STM32s interfacing with a wireless network of other STMs or a server to collect some data. I learned a lot, but I feel like I didn’t do enough to show for it in labs.


### 10-301 Introduction to Machine Learning

This class was probably my favorite class this semester. 10-301 this semester was taught by Gormley, who I found to be an engaging lecturer. Lectures were typical high-level explanations of ML concepts and algorithms, occassionally interrupted with a silly activity that Gormley came up with. Difficulty was on-par with 15-122, due to its similarity in course structure as well as conceptual difficulty. The course is a breadth course, covering topics from all over machine learning such as decision trees, neural networks, hidden Markov models, reinforcement learning, MLE/MAP, and bagging/boosting.

Graded assignments consisted of midterms and homeworks, with a written and programming portion. For the second half of the class (around when probabilistic frameworks are introduced), writtens are conceptually harder than the programming assignments. On the other hand, the hardest programming assignment is probably coding a decision tree classifier from scratch. Otherwise, both written and programming homeworks are relatively straightforward.

Overall, what this course taught was the power of these algorithms that could predict with reasonable accuracy given enough data. A lot of problems in real life that have no straightforward algorithm (such as recommendation or text generation) can be structured as problems in machine learning, and be solved efficiently to some degree. The only (minor) complaints I have with this class is that a lot of the material can be a little vague/unmotivated due to course content structure being all over the place, and that several different notations are used (notably probability and matrix algebra) which can be confusing.


### 18-290 Signals and Systems

This class primarily discusses properties of signals, convolutions, and Fourier Transforms. Devising systems to process signals is only discussed towards the end of the semester. Lectures are extremely boring, as they are 1h 50m, two times per week, with content covered at a snail’s pace. The content, however, was somewhat interesting.


### 76-270 Writing for the Professions

I took this class to fulfill a gen-ed requirement. Extremely light class, and developed some professional skills while taking it. I would recommend this course for anyone trying to learn something light that is useful for their career.