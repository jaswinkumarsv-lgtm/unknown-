IKS MCQ PRACTICE WEBSITE
========================
Files (keep all four in the SAME folder):
  index.html      - the website (design + all functions)
  questions.js    - all 252 questions; index.html loads this file
  questions.json  - backup copy of the same questions
  README.txt      - this file

HOW TO USE
- Open index.html in Chrome. Tap a topic button (T1, T2 ...) to see all its questions on one page.
- Tap an option: green = correct, red = wrong. The correct answer is always shown, and the question locks.
- "Reset" under a question retries only that question.
- "Reset Topic" clears the current topic. "Reset Everything" clears all topics.
- Accuracy = correct answers / attempted questions.
- Progress is saved in your browser (localStorage). Clearing browser data clears progress.
- Topic numbers follow the PDF's lesson numbers. The PDF has no Lesson 18, so there is no T18.

EDITING QUESTIONS
Edit questions.js (and keep questions.json in sync). Each question looks like:
  {"id": 1, "q": "Question text", "options": ["A text","B text","C text","D text"], "answer": "B"}

PUBLISH ON GITHUB PAGES (Android phone, Chrome)
1. Sign in at github.com. Tap + (top right) > New repository.
2. Name it iks-mcq, choose Public, tap Create repository.
3. Tap "uploading an existing file". Tap "choose your files" and select
   index.html, questions.js, questions.json, README.txt (select all four).
4. Wait for the upload bar to finish, then tap Commit changes.
5. Open the repository > Settings > Pages (under "Code and automation").
6. Under Build and deployment: Source = "Deploy from a branch".
   Branch = main, folder = / (root). Tap Save.
7. Wait 1-3 minutes, refresh Settings > Pages. Your link appears:
   https://YOUR-USERNAME.github.io/iks-mcq/
Tip: if the page looks old after an update, hard refresh or open it in a private tab.
