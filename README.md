🧠 Basic & Conceptual Questions
1. What’s the difference between == and === in JavaScript?
Answer: == compares values after type coercion, whereas === compares both value and type without coercion.
Example:

js
Copy
Edit
'5' == 5     // true  
'5' === 5    // false
2. Explain the concept of the Virtual DOM.
Answer: The Virtual DOM is a lightweight copy of the real DOM used in libraries like React. When the state changes, a new Virtual DOM is created and compared to the previous one (diffing). Only the changed parts are updated in the real DOM, improving performance.

3. What are RESTful APIs?
Answer: RESTful APIs follow REST architecture principles — stateless communication, use of standard HTTP methods (GET, POST, PUT, DELETE), and resource-based URLs.
Example: GET /users/1 retrieves user with ID 1.

4. What’s the difference between localStorage, sessionStorage, and cookies?
Answer:

localStorage: persists until manually cleared, ~5MB limit.

sessionStorage: clears on tab close, ~5MB limit.

cookies: sent with every HTTP request, used for auth/session; ~4KB limit.

5. How do you optimize a website’s performance?
Answer:

Lazy loading images

Minifying CSS/JS

Using CDNs

Caching strategies

Reducing API calls

Code splitting

Server-side rendering

🧩 Coding/Logic Questions
6. Reverse a string in JavaScript
js
Copy
Edit
function reverseString(str) {
  return str.split('').reverse().join('');
}
7. Create a simple API using Express.js
js
Copy
Edit
const express = require('express');
const app = express();

app.get('/api/hello', (req, res) => {
  res.json({ message: 'Hello, world!' });
});

app.listen(3000, () => console.log('Server running on port 3000'));
8. Write a responsive grid layout in CSS
css
Copy
Edit
.grid-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 1rem;
}
💡 Behavioral / Real-world Scenario Questions
9. How would you debug a broken UI after a deployment?
Answer:

Check browser console for errors

Inspect network requests in dev tools

Rollback to previous version (if needed)

Check logs or monitoring dashboards

Test in incognito to rule out cache issues

Collaborate with QA/devops if infra-related

10. Tell me about a web app you’ve built. What tech stack did you use?
(Tailor this to your project — e.g., ValetX, Olympics Dashboard, etc.)
Example Answer:
I built a React Native app for smart valet parking called ValetX. It uses real-time QR scanning and OCR to streamline car handovers. Backend is built in FastAPI, uses AWS for image storage, and Firebase for notifications.
