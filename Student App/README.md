# Attendify student app

The Flutter mobile app for students. After logging in, a student sees a dashboard with their attendance, their courses and course details, and their full attendance history. It talks to the same FastAPI backend as the web app.

## Stack

Flutter (Dart 3) · Riverpod for state · Dio for HTTP · flutter_secure_storage for the login token

## Run it

You need the Flutter SDK and the backend running (see the main README).

```bash
cd "Student App"
flutter pub get
flutter run
```

The backend address is set in `lib/config/api_config.dart`. It currently points to an old deployment that is no longer running, so change the URL it returns before running:

- Android emulator: `http://10.0.2.2:8000`
- Browser or desktop: `http://localhost:8000`
- Physical phone on the same Wi-Fi: `http://<your computer's IP>:8000`

## Screens

`lib/views/`: splash, login, dashboard, courses, course details, attendance history.
