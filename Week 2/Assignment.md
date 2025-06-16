# Week 2 Assignment: Build a Mini YouTube Clone (Frontend Only)

## Objective

Create a **basic frontend-only YouTube-like video listing site** using **React JS**. Your goal is to mimic the layout and structure of YouTube’s homepage — video cards, navbar, sidebar (optional), and a search bar UI. The project will help you learn how to use **components, props, hooks (like useState/useEffect), and flexbox/grid layouts** with CSS or Bootstrap.

---

## Core Requirements

> Your website must meet **all** of the following:

### Layout

- A **Navbar** with a YouTube-like title/logo and a dummy search bar
- A **Video Feed section** displaying multiple **video cards** (use an array of dummy video data with props)
- Each **Card** should include:
  - Thumbnail (you can use placeholders or real images)
  - Video title
  - Channel name
  - Views + Time info (for e.g. 1.2M views · 2 days ago)
- The video cards should be aligned using **Flexbox** or **CSS Grid**
- A **Footer** (optional, but encouraged). The footer is optional but good practice for completeness. (For e.g. © 2025 YourName. Built with React.) It can include:
  - Your name or team name
  - A copyright line
  - Social media links (dummy)
  - A link to your GitHub repo

### React Concepts

- **Functional Components** must be used throughout
- Use **props** to pass data to card components
- Use **useState** to toggle dark/light mode or other small stateful features
- Use **useEffect** + **setInterval** to show a **live updating timer** on the page (like “Time Spent on this site: X seconds”). It can be placed at the top or bottom or anywhere you find good. "This timer tracks how long you've been exploring videos — try not to binge-watch for too long!!" 

### Folder Structure

Follow basic good practices:

<pre> src/
├── components/
│   ├── Navbar.jsx
│   ├── VideoCard.jsx
│   └── Timer.jsx
├── data/
│   └── dummyVideos.js
├── App.jsx
└── index.js </pre>


---

## Bonus (Optional but Impressive)

- Add a **Sidebar** similar to YouTube’s (Home, Shorts, Subscriptions etc.)
- Add a **Filter bar** on top (Trending, Music, News...) with button highlights
- Add **Dark/Light Mode toggle** using state
- Make layout **responsive** for mobile and tablet views
- Add a simple **hover animation** on cards (e.g., zoom in thumbnail)

---

## Sample Dummy Data (dummyVideos.js)
```js
export const videos = [
  {
    id: 1,
    title: "React Hooks Explained",
    channel: "CodeWithYou",
    views: "1.2M",
    time: "2 days ago",
    thumbnail: "https://via.placeholder.com/300x170",
  },
  {
    id: 2,
    title: "Flexbox in 10 minutes",
    channel: "CSSNinjas",
    views: "860K",
    time: "1 week ago",
    thumbnail: "https://via.placeholder.com/300x170",
  },
  // add more...
];
```
You may generate and use placedholders from [here](https://smalldev.tools/placeholder-image-generator-online)

## Deadline and Submission
- Submit by Deadline
- Push code to GitHub and share the link on the form we will provide.
- Also make a video of all the features of the site and upload that in the form too.

## Notes
- You can use **Bootstrap** or **Tailwind** for styling — just mention what you used.
- Make sure **everything runs without errors**
- Keep the app simple, aesthetic, and functional

Good luck! Feel free to ask doubts. Let’s build something cool 
<p align="center"> Created with ❤️ by WnCC </p>
