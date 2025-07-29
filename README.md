
# 🌿 Calmly – Minimalist Meditation & Sleep Sounds App  

**Calmly** is a clean, minimalist Android app designed to help users relax and sleep better by listening to ambient sounds.  
This project was built as part of an internship assignment and demonstrates strong Android development skills using **Kotlin, MVVM architecture, Foreground Services, and Material UI design**.

---

## ✨ Features

- 🎧 **Meditation Tab** – Forest, Rain, Ocean, and Campfire ambient sounds  
- 🌙 **Sleep Tab** – White Noise, Lullaby, Fan, Deep Hum & more  
- 🔁 **Looped playback** – High-quality sounds play seamlessly in the background  
- 🛑 **One sound at a time** – Automatically stops the previous sound when a new one starts  
- 🔔 **Foreground Media Service** – Persistent notification with **Play/Pause/Stop** controls  
- 🎨 **Minimal Material Design UI** – Clean, clutter-free user experience  

---

## 🖼️ Screenshots

<p align="center">
  <img src="screenshots/meditation_tab.png" width="30%" />
  <img src="screenshots/sleep_tab.png" width="30%" />
  <img src="screenshots/notification_controls.png" width="30%" />
</p>

---

## 🏗️ Tech Stack

- **Language:** Kotlin (100%)
- **Architecture:** MVVM (ViewModel + LiveData/StateFlow + Repository)
- **UI:** Material Design, RecyclerView, CardView, ViewPager2, BottomNavigationView  
- **Audio:** MediaPlayer + Foreground Service  
- **Asynchronous:** Coroutines + StateFlow  
- **Tools:** Android Studio, Gradle  

---

## 📂 Project Structure (MVVM)

```

com.mehru.calmly/
├─ ui/                # Fragments, Adapters, MainActivity
├─ vm/                # ViewModels
├─ data/              # Repositories (Sound + Playback)
├─ domain/model/      # SoundModel, PlaybackState
├─ playback/          # MediaPlaybackService + PlayController
└─ res/               # Layouts, Drawables, Audio files

````

---

## ⚡ How It Works

1. User selects a sound → `SoundViewModel` triggers **PlaybackRepository**  
2. `PlaybackRepository` communicates with **Foreground MediaPlaybackService**  
3. **Service** handles looping playback, stops previous sounds, and shows **media-style notification**  
4. UI state is updated via **StateFlow** so both Meditation and Sleep tabs stay in sync  


---

### 👨‍💻 Developed by

**Meharban Alam**
📧 [meharban@example.com](mailto:meharban@example.com) | [LinkedIn](#) | [GitHub](#)
