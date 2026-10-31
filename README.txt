1) أنشئ مشروع Firebase، وفعّل Authentication > Anonymous، وأنشئ Firestore Database.
2) انسخ بيانات الويب إلى firebase-config.js.
3) Firestore > Rules:
   rules_version='2'; service cloud.firestore { match /databases/{d}/documents { match /rooms/{id} { allow read, write: if request.auth != null; } } }
4) ارفع محتوى المجلد على GitHub.
5) للتحديثات: زوّد الأسئلة في questions.js فقط.
