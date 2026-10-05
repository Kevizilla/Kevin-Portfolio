# Kevin Stephen — Portfolio

A responsive personal portfolio website built with **HTML, CSS, and JavaScript** to showcase my profile, skills, projects, and contact information.

## Overview

This project is a simple, dark-themed portfolio designed to present my work and learning journey as a student developer.

The website focuses on a clean interface, responsive layouts, and a few interactive JavaScript features that improve the user experience.

## Features

* Responsive portfolio layout for desktop, tablet, and mobile
* Sticky navigation bar
* Section-based navigation using HTML `id` and anchor links
* Active navigation link highlighting while scrolling
* Animated skill bars
* Back-to-top button with smooth scrolling
* Responsive project and information cards
* Custom background grid created using CSS gradients
* Google Fonts integration
* Contact section with email link

## Technologies Used

### HTML

* Semantic elements such as `header`, `nav`, `main`, `section`, and `article`
* Anchor links for navigation
* Custom `data-width` attributes for skill bars

### CSS

* CSS variables for consistent colours
* CSS Grid and Flexbox for layouts
* Responsive design using media queries
* CSS transitions for animations
* Linear gradients for the background grid

### JavaScript

* DOM selection using `querySelectorAll()` and `getElementById()`
* Scroll event listeners
* Active navigation highlighting
* Back-to-top functionality
* `IntersectionObserver` for skill-bar animation
* `dataset` for reading custom HTML attributes

## JavaScript Functionality

### Active Navigation

The website detects which section is currently being viewed while scrolling.

`getBoundingClientRect()` is used to determine the position of each section, and the corresponding navigation link receives the `active` class.

### Back to Top

The back-to-top button appears after the user scrolls more than 400 pixels.

When clicked, `window.scrollTo()` smoothly moves the page back to the top.

### Skill Bar Animation

Each skill contains a `data-width` attribute that stores its target percentage.

When the Skills section enters the viewport, an `IntersectionObserver` triggers the animation. JavaScript reads the stored value using `dataset.width` and assigns it to the bar's CSS width.

The CSS `transition` property makes the change animate smoothly.

## Project Structure

```text
portfolio/
│
├── index.html
├── styles.css
├── profile.png
└── README.md
```

## Running Locally

1. Clone the repository:

```bash
git clone <repository-url>
```

2. Open the project folder:

```bash
cd portfolio
```

3. Open `index.html` in a browser.

No additional dependencies or build tools are required.

## Deployment

The website is deployed using **Netlify**.

Whenever changes are made to the project, the updated files can be redeployed to Netlify.

## Project Sections

The portfolio contains:

* **Home** — Introduction and profile
* **About** — Background and areas of focus
* **Skills** — Technical skills and proficiency bars
* **Projects** — NEXUS, the portfolio itself, and competitive programming practice
* **Highlights** — A few project and learning statistics
* **Contact** — Email contact information

## Author

**Kevin Stephen**

Student Developer
Scaler School of Technology
