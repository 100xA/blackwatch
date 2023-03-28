---
layout: post
title: Project "Zample"
description: Notes on the Project "Zample" - a Cross-Plattform Application for centrally distributing ideas and their respective creators.
comments: false
tags: [java.dart, flutter, firebase, status-finished]
---

# General Info

The Application "Zample" is a Cross-Plattform Application for centrally distributing ideas and their respective creators.

Since 2019, the program has been developed by myself and two other team-members, with the goal to ease the way how people share very early ideas and provide a fresh marketplace for them.

![Zample Design](/assets/images/zample-design.png){:.align-center}


# Technical Summary  

"Zample" is written with the **Flutter/Dart Cross-Plattform** Framework created by Google.
The Projects Database is maintained by **Google Firebase**. 

To have a clear and functioning seperation between UI, BL and Repository, the popular state management library **BLoC/Cubit (Business Logic other Component)** was chosen.
Cubit, being an extension of the BLoC library, is often used to better organise the BL's `BlocBase`.

![BLoC/Cubit](/assets/images/bloc-cubit-arch.png){:align-center}

To ensure easy dependency injection, the package [`get_it`](https://pub.dev/packages/get_it) was used. Services across the application can now be implemented/referenced/called from everywhere in the project.

## Project Structure


```
├── lib
│   ├── api
│   ├── components
│   │   ├── home
│   │   │   ├── bloc
│   │   │   │   └── cubit
│   │   │   └── ui
│   │   ├── landing
│   │   │   ├── bloc
│   │   │   │   └── cubit
│   │   │   └── ui
│   │   │       └── widgets
│   │   ├── profile
│   │   │   ├── bloc
│   │   │   │   └── cubit
│   │   │   ├── repo
│   │   │   └── ui
│   │   │       └── widgets
│   │   └── settings
│   ├── core
│   │   ├── bloc
│   │   │   ├── app
│   │   │   ├── auth
│   │   │   └── theme
│   │   ├── error_handler
│   │   ├── logger
│   │   ├── repo
│   │   ├── services
│   │   └── widgets
│   ├── main.dart
│   ├── misc
│   │   ├── routes
│   │   └── theme
└── test
```

The Project follows the principles of dividing UI/BL/Repository, while incorporating some aspects of the `Clean Architecture`-approach.

* **Api** - Endpoints to every API that has been used
* **components** - Main components of the application, divided into each functional part of the application, where every part has a own UI/BL/Repository for its service
* **core** - overarching features of the application (authentication, logging etc.)
* **misc** - miscellanous features (routing, themes/color schemes) of the application
* **test** - folder for test for the application (not included in the project)

# Links and further information

* [Link to the repository](https://github.com/100xA/Zample)
* [Link to the website on Notion](https://pstarterapp.de)

The project is no longer active.