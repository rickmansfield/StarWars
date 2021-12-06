# ReactWars
![Star-Wars-Mock](src/images/sw-bg.jpg)

This challenge allowed me to practice the concepts and techniques Javascript combined with React and apply them in a concrete project. This sprint explored **introductory React**. During this sprint, I studied **React components and advanced styling**.

Here I demonstrate mastery of these skills by creating **a Mock Star Wars page** using data from an API.
## About The Author Rick Mansfield
## [Visit this live site](https://mansfield-port-v3.netlify.app/)
### Hi there 👋

<!--
**rickmansfield/rickmansfield** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 😄 Pronouns: ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- ⚡ Fun fact: ...
-->
- 💬 Ask me about coding and I may never shut up. LOL
- 📫 How to reach me: [Resume](https://resume.creddle.io/resume/4uxc0m7zngm) or [LinkedIn](https://www.linkedin.com/in/peacefulrick/)
- 😄 [See My PORTFOLIO](https://mansfield-port-v3.netlify.app/)
- ⚡ Fun fact: ...really wanted to obtain the domain name VikingsCode.com since my family descended from Germanic Vikings!

## Skills:
### FRONTEND: 
- React.js, Redux, Hooks, Context API, Jest, Yum, Axios, Javascript, HTML, CSS, Ant Design, RESTful API Design, JSX
### BACKEND:
- Node.js, Express, SQL, PostgreSQL, Python, Git CLI, VS Code, Vercel, Heroku, Netlify, Postman
### ADDITIONAL SKILLS:
- Agile Project Management, Algorithms, Architecture, Debugging, Deployment, Technical Project Management
## Want to build this yourself? Project Set Up

- [ ] Fork and clone the repo. 
- [ ] ```npm install```
- [ ] ```npm start ```
- [ ] Push your first commit: `git commit --allow-empty -m "first commit" && git push`.

## Project Instructions

### Introduction

In this demo I create a web page that presents a styled list of characters obtained from an API. Being able to render out data to a web page is a large part of what JavaScript developers do, this challenge demos the ability to achieve such a task.

### Instructions

This finished project includes all of the following:

- [ ] Use of the endpoint `[GET] https://swapi.dev/api/people` (mocked in [msw](https://github.com/mswjs/msw)) to obtain characters.
- [ ] Set the list of characters into state.
- [ ] Rendered characters to the DOM:

### Want to build this yourself? 
  1. Build a React component named 'Character' to render an individual character.
  2. Map over the list in state, and for each character render a Character to the page.
  3. Each rendered character must display its name in the DOM (e.g. "Luke Skywalker").
  4. The character's name can't be hard-coded into the HTML. This data must be obtained from the API.
  5. The components must be styled with **styled-components**.

  **Notes:**

- Data obtained from the endpoint using browser-run JavaScript is mocked with [msw](https://github.com/mswjs/msw).
- If you test the endpoint using HTTPie or Postman you will obtain different results, as msw won't intercept the request.
- Do not alter your `package.json` file except to install extra libraries.
- The `start` process can sometimes choke after adding new dependencies and may need to be restarted.
- In your solution, it is essential that you follow best practices and produce clean and professional results.
- Schedule time to review and polish your work, including spell-checking and grammar-checking.
### Stretch Goals

After finishing your elements, you can push your work further, stretch your limits and see if you can deliver on any the following optional goals:

- [ ] Make the Character component more complex and break it into several subcomponents.
- [ ] Use the endpoint `[GET] https://swapi.dev/api/films` (mocked in msw) to obtain movie information to render with the characters.
- [ ] Create a helper function in separate module to remove unneeded information from the API data, before putting it in state.
- [ ] Create transitions or animations with styled-components.
- [ ] Use Promise.all to resolve an array of promises.

## Notes for Interview Questions

Be prepared to demonstrate your understanding of these concepts by answering questions on the following topics. You might prepare by writing down your own answers before hand.

1. What is React JS and what problems does it solve? Support your answer with concepts introduced in class and from your personal research on the web.

**Answer** 
After reviewing [React](https://reactjs.org/) they say it's a Javascript library for building user inerfaces. In my own words, React.js is an open-source JavaScript Library. It is not a language. It's used to build out DOM from within a JS file specifically for single-page type applications giving a smooth fast user interface. It's scalable and it makes both the front end developer job and UX optimal. Let's pat Mark Zuckerburg's Jordan Walke (software engineer) on the back for making our lives easier.

2. Describe component state.

**Answer**
"State is a JavaScript object holding information that affects render output and it is managed withing a component similar to variables being declared in a function. (On/off, True/false, and booleen examples.)

3. Describe props.

**Answer**
Props is short for "properties" and like state is also a plain JavaScript object. It also holds information that affectst the output render but unlike state props gets passed to the component sort of like function parameters. 

4. What are side effects, and how do you sync effects in a React component to changes of certain state or props?

**Answer**
"Side Effects" are anything that affects something outside the scope of the function being executed. Examples: fetching api data, timers, logging, and manual DOM manipulations. The come in two flavors those requiring cleanup and those that don't. We sync effects in a React componenet using tools like The **Effect Hook**. Using a dependency array as the second argument in the effect hook, we can tell it with which state or props the effect should be synced. I like this handy summary
- useEffect(fn); // all state and props
- useEffect(fn, []); // no state or props
- useEffect(fn, [these, states, props]);
