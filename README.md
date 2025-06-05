# Actual Useful Assistant

**A cross-platform personal assistant combining GUI, CLI, and mobile interfaces to boost productivity, learning, and well-being.**

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Why Build This?](#why-build-this)
3. [Supported Platforms](#supported-platforms)
4. [Core Features](#core-features)
   - [1. Task & Time Management](#1-task--time-management)
   - [2. AI-Driven Assistance](#2-ai-driven-assistance)
   - [3. Learning & Skill-Building](#3-learning--skill-building)
   - [4. Motivation & Well-Being](#4-motivation--well-being)
   - [5. Journaling & Reflection](#5-journaling--reflection)
   - [6. Personalization & Memory](#6-personalization--memory)
5. [Technology Stack](#technology-stack)
6. [Getting Started](#getting-started)
7. [Future Roadmap](#future-roadmap)

---

## Project Overview
**Actual Useful Assistant** is designed to be a one-stop solution for:
- Managing tasks, schedules, and goals  
- Enhancing creativity and learning with AI-driven tools  
- Tracking motivation, well-being, and work-life balance  
- Providing both GUI (desktop/mobile) and CLI interfaces for flexibility  

It merges productivity, mental health considerations, and continuous learning into a seamless experience—accessible on macOS (native app), Windows/Linux (CLI), and Flutter-based mobile applications (Android & iOS).

---

## Why Build This?
1. **Unified Productivity Hub** (so you don’t need multiple apps for tasks, scheduling, journaling, and motivation).  
2. **AI-Powered Intelligence** (leveraging Gemini APIs to handle language tasks, suggestions, and personalized interactions at no extra cost).  
3. **Cross-Platform Convenience** (CLI for quick terminal enthusiasts; GUI for point-and-click usability; Flutter-based mobile app for on-the-go access).  
4. **Data-Driven Well-Being** (tracking scores, analyzing trends, avoiding burnout, and promoting healthy habits).  
5. **Open & Extensible** (built with Firebase backend—easily extendable and self-hostable with user-provided API keys).

---

## Supported Platforms
- **macOS, Windows App (GUI + Menu Widgets)**  
  - Built with PyQt5 for the main window and Rumps for menu bar widgets/quick access (to leverage Python’s cross-platform libraries and provide lightweight menu features).  
- **Cross-Platform CLI (macOS, Windows, Linux)**  
  - Python-based command-line interface for scripting, automation, and quick-access workflows.  
- **Flutter Mobile App (Android & iOS)**  
  - Syncs seamlessly with desktop versions (shared database via Firebase).  
  - Lightweight interface optimized for touch interaction.

---

## Core Features

> Each feature is grouped by category and includes a brief rationale in brackets.

### 1. Task & Time Management
- **Task Management**  
  - Create, categorize, prioritize, and track tasks (to centralize to-dos and improve focus).  
- **Daily Schedule & Event Planning**  
  - Visualize calendar, set reminders, and map out day-by-day activities (to make each day purposeful and prevent overcommitment).  
- **Time Blocking & Pomodoro/90-Minute Rule**  
  - Block dedicated chunks of time for focused work (to boost concentration and leverage ultradian rhythms).  
- **Priority & Goal Setting**  
  - Define short-term and long-term goals, link tasks to goals (to ensure alignment with personal/professional objectives).  
- **Automatic Task Suggestions**  
  - System analyzes incomplete tasks, deadlines, and priorities to propose what to work on next (to reduce decision fatigue).  
- **Tagging & Smart Filtering**  
  - Tag tasks, notes, and journal entries for robust filtering and search (to quickly locate items and generate analytics).

### 2. AI-Driven Assistance
- **Quick Text Rephrasing**  
  - Leverage Gemini APIs to rephrase emails, documents, or messages (to save time and enhance writing quality).  
- **Chatbot Interface for Task Guidance**  
  - Ask context-aware questions about tasks, workflows, or goals (to receive intelligent recommendations and encouragement).  
- **Auto-Research & Opportunity Seeker**  
  - AI scans news/articles or relevant sources to suggest new tools, trends, or opportunities related to user’s interests (to keep users informed without manual searching).  
- **AI Modes & Profiles**  
  - Switch between “Productivity Mode,” “Creative Mode,” “Learning Mode,” etc., each adjusting AI suggestions and UI focus (to adapt to the user’s current need).

### 3. Learning & Skill-Building
- **Flowchart Creator**  
  - Build visual flowcharts for learning plans, workflows, or processes (to simplify complex concepts and track progress).  
- **Learning Notes & Flashcards**  
  - Take structured notes, generate flashcards automatically from notes (to facilitate spaced repetition and long-term retention).  
- **Idea Sandbox**  
  - Free-form space to jot down ideas, brainstorm, and link related concepts (to encourage creativity and avoid idea loss).  
- **Memory-Based System for Personalization**  
  - Store user preferences (learning styles, frequent tasks, favorite topics) to tailor UI prompts and suggestions (to deliver a more relevant experience over time).

### 4. Motivation & Well-Being
- **Quotes & Motivational Snippets**  
  - Display user-selected or randomized motivational quotes upon launch or at scheduled intervals (to boost morale).  
- **Embedded Video Player for Motivational Content**  
  - Save motivational video links (YouTube, Vimeo, etc.) and play them in-app (to minimize context switching).  
- **Work-Life Balance Score**  
  - Analyze logged work hours vs. personal/leisure time, provide a numeric score (to prevent burnout and maintain healthy boundaries).  
- **Day Score & Burnout Analysis**  
  - Rate each day’s difficulty (Very Easy → Very Hard), track weekly/monthly trends, and give recommendations when signs of burnout appear (to proactively protect mental health).  
- **Notification & Reminder System**  
  - Desktop push notifications (via Rumps), system tray icons, and mobile push alerts for important tasks and journaling prompts (to keep users on track).

### 5. Journaling & Reflection
- **Daily Journaling**  
  - At the end of each day, prompt user to write reflections, lessons learned, and emotional check-ins (to encourage self-awareness and mindfulness).  
- **End-of-Day Revision & RAM Clearing**  
  - Quick “brain dump” section for dangling thoughts (to free mental bandwidth and reduce anxiety).  
- **Progress Reports**  
  - Weekly/Monthly summary of tasks completed, goals achieved, learning milestones, and well-being metrics (to review achievements and identify areas for improvement).

### 6. Personalization & Memory
- **User Profiles & Preferences**  
  - Store user’s preferred themes, notification settings, time-zone, and preferred work rhythms (to deliver a consistent, tailored experience).  
- **Adaptive UI**  
  - Rearrange dashboard widgets based on usage patterns (to surface frequently used features without manual configuration).  
- **Customizable AI Prompt Templates**  
  - Users can define default prompts or templates for tasks like email drafting, research queries, or reflection journaling (to speed up repetitive activities).  
- **Database Sync via Firebase**  
  - Real-time syncing between desktop (PyQt5/Rumps), CLI, and mobile (Flutter) (to keep data consistent across devices).  
- **Offline Support (Cache Mode)**  
  - Allow basic task management and journaling offline, then sync when connectivity is restored (to maintain productivity in low-connectivity scenarios).

---

## Technology Stack

- **Front-End GUI (macOS, Windows)**:  
  - **PyQt5** for the main window (leveraging Qt’s cross-platform GUI toolkit).  
  - **Rumps** for macOS menu bar widgets and quick-access controls (to provide lightweight system integration and notifications).  

- **CLI (macOS, Windows, Linux)**:  
  - Written in Python (using [Click](https://click.palletsprojects.com/) or [Typer](https://typer.tiangolo.com/) for argument parsing).  
  - Supports scripting, alias setup, and custom user commands.

- **Mobile (Android & iOS)**:  
  - Flutter (single codebase for both platforms).  
  - Firebase Authentication + Firestore for data sync.

- **Backend / Database**:  
  - **Firebase Firestore** (NoSQL) for real-time data sync, authentication, and storage (so users can self-host with their own Firebase project).  
  - **Gemini API** (for free-tier AI tasks like rephrasing, chat suggestions, flowchart generation prompts).

- **Video Player Integration**:  
  - For macOS GUI: integrate a PyQt5-based media player widget (e.g., QtMultimedia).  
  - For Flutter: [video_player](https://pub.dev/packages/video_player).

- **Analytics & Charts**:  
  - Use Python plotting libraries (e.g., matplotlib) to generate analytics charts in the PyQt5 GUI.  
  - In Flutter, use packages like [charts_flutter](https://pub.dev/packages/charts_flutter) for in-app visualizations.

---

## Getting Started

1. **Clone the Repository**  
   ```bash
   git clone https://github.com/your-username/actual-useful-assistant.git
   cd actual-useful-assistant
