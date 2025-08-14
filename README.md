# Birthday Reminder (Android, Kotlin, Jetpack Compose)

Features:
- Store Name, Nickname, Birthdate (YYYY-MM-DD), Photo.
- List view with photo.
- Share message: "Happy Birthday <nickname> 🎉" (opens WhatsApp if available, else system share).
- Daily 9:00 AM notification if any birthday matches today's date (by month/day).
- Data stored locally using Room.
- Photo chosen via *Open Document* (no storage permission needed).

## Build
1. Open this folder in **Android Studio (Giraffe+ / latest)**.
2. Let Gradle sync. If prompted, install missing components.
3. Run on device or **Build > Build APK(s)** to generate an APK.

Notes:
- On Android 13+, the app will ask for the **POST_NOTIFICATIONS** permission at first notification; allow it.
- Keep the app installed; WorkManager will run daily. If phone reboots, it will reschedule automatically.
