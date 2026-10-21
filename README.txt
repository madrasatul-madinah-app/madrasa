ধাপ ১ (GitHub-এ আপলোড)
- github.com → New repository → নাম: madrasa → Public → Create
- "uploading an existing file" চাপুন → এই ZIP থেকে সব ফাইল টেনে দিন (index.html সহ) → Commit changes

ধাপ ২ (ওয়েবসাইট চালু)
- repository → Settings → Pages → Branch: main, Folder: /(root) → Save
- ১-২ মিনিট পর লিংক পাবেন: https://আপনার-নাম.github.io/madrasa/

ধাপ ৩ (Firebase - ডেটা সিঙ্ক)
- console.firebase.google.com → Add project
- Build → Authentication → Get started → Sign-in method → Anonymous → Enable
- Authentication → Settings → Authorized domains → Add: আপনার-নাম.github.io
- Build → Firestore Database → Create database (production mode)
- Firestore → Rules ট্যাব → firestore.rules ফাইলের লেখা পেস্ট করে Publish
- Project settings (গিয়ার) → Your apps → Web (</>) → Register → firebaseConfig-এর { ... } অংশ কপি
- এপ খুলে: আরও → ক্লাউড সিঙ্ক → পেস্ট → চালু করুন
