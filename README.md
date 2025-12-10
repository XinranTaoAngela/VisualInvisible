# Visual Invisible

**An Invisible Wellness Companion for Students — iOS Prototype (SwiftUI)**

Visual Invisible is an experimental iOS prototype designed to support students' productivity, emotional awareness, and daily wellness, without requiring the user to constantly interact with the app.

The core idea is simple: An AI-powered wellness companion that works quietly in the background — tracking habits, prompting intentional usage, and helping users maintain balance. This prototype is fully implemented in SwiftUI, designed to run in the iOS Simulator as a concept demo.

> No backend, no API keys — lightweight and fully local.

## ✨ Core Features

### 1. 🎯 Intention Interception for Distracting Apps

When users tap on apps like TikTok, Instagram, or YouTube (simulated inside the prototype), the app gently asks:

**"Why are you opening this?"**
- Rest
- Research / inspiration  
- Just scrolling

This promotes mindful technology use and reduces automatic distraction.

---

### 2. 🫧 Global Double-Tap Quick Log (Anywhere in the App)

Users can double-tap anywhere on the screen to instantly open a Quick Log panel:
- 🥤 Log a cup of water
- 🏃 Add 10 min of physical activity
- 🙂 Log a positive mood

This interaction models a "background companion" behavior — users don't need to navigate to a specific page.

---

### 3. 📊 Today Dashboard

A daily summary screen displaying:
- Total focus minutes
- Sleep duration
- Number of distractions today
- Water intake
- Recent activities
- An AI-style wellness summary that describes the user's daily behavior patterns

---

### 4. 😺 Mood Reflection Slider

Users record their emotional state on a 1–5 scale with emoji anchors.  
This contributes to the daily summary and wellness trend.

---

### 5. 📱 Simulated iPhone Home Screen

To demonstrate behavior interception, the prototype includes a fake iPhone home screen with tappable TikTok/Instagram icons.  
This lets us test intention-logging without requiring real OS-level API hooks.

---

## 🎯 Motivation

Modern students struggle balancing:
- Productivity
- Mental health
- Digital distraction
- Wellness habits

Visual Invisible explores how an AI system could intervene subtly, gently, and intentionally, without being intrusive.

Rather than a traditional "open app → track habit," this prototype imagines a system that:
- Listens passively
- Surfaces just-in-time nudges
- Helps users build healthy routines effortlessly

---

## 🛠 Built With

- **SwiftUI** (iOS 17+)
- **Xcode** (prototype only)
- **MVVM-style** state container with `ObservableObject`
- **SwiftUI** Sheets, TabView, and Gestures
- Fully local state (no external frameworks needed)

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/VisualInvisible.git
   ```

2. Open the project in Xcode 15+

3. Select an iOS simulator (e.g., iPhone 16 Pro)

4. Run using `⌘ + R`

---

## 📐 Architecture

```
VisualInvisibleApp.swift       → App entry point
ContentView.swift              → Main UI logic (RootView, gesture layer, QuickLog sheet)
WellnessState.swift            → Data model + state container
SimulatedHomeScreen.swift      → Fake iPhone launcher
TodayDashboard.swift           → Daily summary view
MoodView.swift                 → Mood tracking page
IntentionSheet.swift           → Distraction interception modal
```

All behavior is local and state is stored in-memory for demo purposes.

---

## 📚 Future Extensions (Planned Ideas)

- **Real-time HealthKit integration** (sleep & steps)
- **Focus Session Timer** with automatic interruption logging
- **Weekly trend analytics** (mood → habits correlation)
- **AI-generated insights** using simple rule-based or LLM prompts
- **Customizable Quick Log actions** (water, stress level, meditation)
- **Push notifications** for hydration or rest

---

## ⭐ Why This Project Matters

This prototype blends:
- **HCI principles**
- **Behavioral psychology** (nudging)
- **AI-assisted well-being**
- **Minimal UI, maximum impact**

It demonstrates how digital well-being tools can be proactive, context-aware, and emotionally supportive—without being annoying or demanding.
