$readme = @'
# DeutschGo

Online platform for learning German, built with Flutter (web) and Firebase.

## Features
- Interactive lessons: phrases, dialogues, matching, listening, fill-in and sentence building
- Explanations in English, Arabic and Somali
- Exam practice program with a 30-day plan
- Teacher voice recording and text-to-speech audio
- Subscriptions with online payments (Paystack) and manual M-Pesa approval
- Admin panel for levels, units, lessons and exams

## Tech
Flutter Web, Firebase (Auth, Firestore, Storage, Cloud Functions, Hosting), Google Cloud Text-to-Speech, Paystack.

## Setup
1. Install Flutter and the Firebase CLI.
2. Create a Firebase project and run `flutterfire configure` to generate `lib/firebase_options.dart` (not included in this repository).
3. Store secrets with `firebase functions:secrets:set PAYSTACK_SECRET_KEY` (never commit keys).
4. Run `flutter run -d chrome`.

## License
All rights reserved. The code and course content may not be copied or reused without permission.
'@
[System.IO.File]::WriteAllText("$PWD\README.md", $readme, (New-Object System.Text.UTF8Encoding $false))# Germen-learning-Web
A German language learning website offering structured lessons from A1 to B1, interactive exercises, mock exams, and learning resources for students.
