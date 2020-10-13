---
title: "Drivers exam"
layout: post
date: 2020-09-11 15:00
tag: flutter, dart, ui
headerImage: false
projects: true
hidden: true # don't count this post in blog pagination
description: "Unofficial application for NCC car, motorcycle and animal exam."
category: project
author: riccardo
externalLink: false
---
<span class="project-used-item">Dart & Flutter</span>
<span class="project-used-item">Clean architecture</span>
<span class="project-used-item">Firebase </span>
<span class="project-used-item">Notifications</span>
<span class="project-used-item">Internal SQL database</span>
<span class="project-used-item">iOS & Android</span>
<span class="project-used-item red-project">Closed source <span class="ec-lock"></span></span>
<span class="project-used-item green-project">In beta testing <span class="ec-hammer"></span></span>

Unofficial application for NCC car, motorcycle, and animal exam. With this application, you can practice the tests to get the NCC license. The NCC license enables you to drive vehicles for a rental service.


To get the questions and answers I obtained all the data from pdf files of the region, then I entered the data in a Firestore database, so I'm able to update the questions and answers.

The stack I used:
- **Mobile application**: flutter & dart
    - **state managment**: BLoC
    - **database**: moor
    - **notifications**: FCM
    - **fetching from remote**: Firebase

- **Obtaining the data**: python for scraping the data from the pdfs
    - **pdf library**: PyPDF2

<br>
I developed this app without any colleague.


<div style="text-align: center; margin-top: 30px;">
<img src="../../img/featured/esame/multiple-phones.png" alt="phones" />
</div>
