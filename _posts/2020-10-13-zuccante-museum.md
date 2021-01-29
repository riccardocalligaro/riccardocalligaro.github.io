---
title: "🏛 Museo Zuccante"
layout: post
date: 2019-11-02 18:00
tag: flutter, dart, ui
headerImage: false
projects: true
description: "Application for the school museum"
category: project
author: riccardo
externalLink: false
---


<span class="project-used-item">Dart & Flutter</span>
<span class="project-used-item">Clean architecture</span>
<span class="project-used-item">Streams & rxdart</span>
<span class="project-used-item">REST API</span>
<span class="project-used-item">Animations</span>
<span class="project-used-item">Internal SQL database</span>
<span class="project-used-item">iOS & Android</span>
<span class="project-used-item green-project">In beta testing <span class="ec-hammer"></span></span>
<span class="project-used-item green-project">Open source<span class="ec-unlock"></span></span>


<h1 align="center">
    <a target='_blank' href='https://github.com/Saerlig-Software-Development/museozuccante_client'><img height="100px" alt='Get it on Google Play' src='../../img/github_button.png'/></a>
</h1>


What I did:
- **Mobile application**: Developed the mobile application for Android and iOS, it was coded with a clean architecture and I used BLoC for managing of the state.


- Riccardo Calligaro -  **Application**
- Filippo Veggo - **Design consultant**
- Leone Bacciu - **Backend (Django + Docker)**
- Diego Caspi - **Backend (Django)**<br>


<div style="text-align: center; margin-top: 30px;">
<img src="../../img/featured/museum/1.png" alt="screen1" width="200"/>
<img src="../../img/featured/museum/2.png" alt="screen1" width="200"/>
<img src="../../img/featured/museum/3.png" alt="screen1" width="200"/>
</div>



<br>

# Documentation

## Libraries
- 🔝  Flutter + Dart
- 📡  Dio for API requests
- 💡  BLoC for state management
- 📚  Foor for data persistency
- 💉  Get It for dependency injection
- 🔗  Dartz for functional programming
- 🌊  RxDart for the data flow

## Handling errors

Error is handling is done with functional programming, every function and streams gives a Either or a Resource type, so in the UI we can give an error message

## What is the Clean Architecture by Uncle Bob?

![The clean architecture](https://miro.medium.com/max/1400/1*wOmAHDN_zKZJns9YDjtrMw.jpeg)

1. Module to present the data. This is called a presentation Layer.
2. Module to get data/feeds from. Can be local(like DB) or Remote(like REST calls). This is called Data Layer.
3. Business logic which shows the feeds/to handle like and dislike. This is called Domain Layer.


## Design patterns
- usecases
- repository
- dependency injection
- observer


## Data

The Data layer consists of repository and data models. Repository is where the application gather all data related to the use case, either from local sources (Local DB, cookies) or remote sources (remote API). Data from the sources, usually in json format, is parsed to Dart object called models. It’s need to be done to make sure the application knows what data and variable it’s expecting.

## Domain

Domain is the inner layer which shouldn’t be susceptible to the whims of changing data sources or porting our app to Angular Dart. It will contain only the core business logic (use cases) and business objects (entities).
Repository classes act as the Data Layer and Domain Layer, each function on the repository class acts as the domain layer that specifies the use cases of the feature.

Domain Layer can have:
1. Use cases
2. Entities
3. DataLayer interfaces



## Presentation
Presentation is where the UI goes. You obviously need widgets to display something on the screen. These widgets is controlled by the state using various state management design pattern used in Flutter. In this project, I use BLoC as the state management.

## Dependencies/Data flow

UI calls from the Presentation layer.
Presentation layer executes the use case.
Use case(Domain layer) will ask the Data layer to send back the result.
Data layer will run and send back the result to the Use case.
Information is flown back to UI, to show the result.


