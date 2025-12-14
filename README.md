# BlackByteJs


⚡ BlackByte JS — Live JavaScript Sandbox & Console

BlackByte JS is a fast, lightweight, browser-based JavaScript sandbox that allows developers to write, run, and debug JavaScript code live while typing, with full support for async/await, fetch API, and real-time console output.

Built from scratch using Vanilla JavaScript, HTML, CSS, and Tailwind CSS, this project focuses on performance, usability, and real-world debugging needs — without relying on heavy editors or external compilers.

🚀 Live Demo (Optional)

https://himanshna.github.io/BlackByteJs/

🧠 Why I Built This

While learning JavaScript deeply, I faced multiple problems with existing online JS editors:

Slow execution

Poor or broken API / fetch support

Async code (async/await) not behaving correctly

No real-time feedback while typing

Overloaded editors that hide what’s actually happening

So instead of adjusting to those limitations, I built my own fast JS sandbox — optimized for learning, testing, and debugging real-world JavaScript.

✨ Key Features

🔴 Live Auto-Run JavaScript (runs automatically while typing)

⚡ Fast execution with debounced evaluation

🌐 Full Fetch API support

⏳ Proper handling of async / await

🖥️ Custom Console Output

console.log

console.error

console.warn

console.info

🧹 Clear Console button for clean debugging

✍️ Clear Editor button for instant reset

▶️ Manual Run Button (Ctrl + Enter supported)

🎨 Glassmorphism UI Buttons

📱 Fully responsive layout

🛑 Global error & promise rejection handling

🛠️ Tech Stack

HTML5

CSS3

Tailwind CSS

Vanilla JavaScript (ES6+)

Async/Await

Fetch API

DOM Manipulation

Event Handling

Debouncing

Eval with Async IIFE

🧩 Problems I Faced & How I Solved Them
1️⃣ Slow Code Execution

Problem:
Initially, code only ran on button click and felt slow during testing.

Solution:
Implemented debounced auto-execution using the input event, ensuring:

Code runs only after typing pauses

No browser freezing

Instant feedback

2️⃣ Fetch API Not Working

Problem:
Many online JS compilers failed to execute API calls properly.

Solution:

Used native browser environment

Wrapped user code inside an async IIFE

Ensured fetch works exactly like real applications

3️⃣ Async / Await Errors

Problem:
async/await caused execution issues and silent failures.

Solution:

Wrapped evaluated code inside:

(async () => { ... })();


Added global error and unhandled promise rejection listeners

4️⃣ No Proper Console Output

Problem:
Default console logs were invisible inside the app.

Solution:

Overrode console.log, error, warn, and info

Created a custom styled console UI

Auto-scroll enabled for better readability

5️⃣ Poor Developer Experience

Problem:
Resetting code/output took too long during testing.

Solution:

Added Clear Editor

Added Clear Console

Added Manual Run Button as a fallback

6️⃣ UI & Visual Polish

Problem:
Basic buttons felt boring and unprofessional.

Solution:

Designed glassmorphism-style buttons

Smooth hover, active, and shadow effects

Clean, distraction-free editor layout

📂 Project Structure
BlackByteJS/
│
├── index.html
└── README.md

🧪 Example Usage
async function getUsers() {
  const res = await fetch("https://jsonplaceholder.typicode.com/users");
  const data = await res.json();
  console.log(data);
}

getUsers();


✔ Runs instantly
✔ Shows output in console
✔ Handles async properly

🎯 Ideal For

JavaScript learners

Frontend developers

MERN stack developers

Debugging API calls

Practicing async/await

Technical interviews & demos

🔍 SEO & ATS Keywords

JavaScript Sandbox, Live JavaScript Editor, Online JS Compiler, Async Await JavaScript, Fetch API JavaScript, Frontend Development, Vanilla JavaScript Project, JavaScript Debugging Tool, Web Developer Portfolio, JavaScript Practice Tool, DOM Manipulation, Tailwind CSS Project, Software Engineering Project

🛣️ Future Improvements (Suggestions Welcome)

Toggle Live Run ON/OFF

Execution time display

iframe-based sandbox isolation

Save code to LocalStorage

Multiple files support

Dark mode

👤 Author

HimAnsh Namdeo
Aspiring Software Engineer | Frontend & MERN Stack Developer
Passionate about building fast, real-world developer tools and learning JavaScript deeply.

📫 Suggestions, feedback, and contributions are always welcome.
