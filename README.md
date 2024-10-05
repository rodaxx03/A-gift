#💐Resource flowers gift website for someone

# Flowers for Someone 🌸

Welcome to Flowers for Someone! 🌼 This repository hosts the codebase for a charming website dedicated to the art of gifting flowers to your loved ones. Express your sentiments with the beauty of nature!

## Table of Contents
- [Introduction](#introduction)
- [Technologies Used](#technologies-used)
- [Installation](#installation)

## Introduction

Flowers for Someone is your ultimate destination for heartfelt floral gifting. Whether it's a special occasion or just to brighten someone's day, our website offers a delightful of flower arrangements, bouquets, and personalized messages.

## Technologies Used

This project utilizes the following programming languages and technologies:
- HTML
- CSS
- SCSS (Sass)
- JavaScript

## Installation

To run this project locally, follow these steps:

1. Clone this repository to your local machine:
 111 changes: 111 additions & 0 deletions111  
wahyu bunga/css/index.css
Original file line number	Diff line number	Diff line change
@@ -0,0 +1,111 @@
*,
*::after,
*::before {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

:root {
  --dark-color: #000;
}

.night {
  position: fixed;
  left: 50%;
  top: 0;
  transform: translateX(-50%);
  width: 100%;
  height: 100%;
  filter: blur(0.1vmin);
  background-image: radial-gradient(ellipse at top, transparent 0%, var(--dark-color)), radial-gradient(ellipse at bottom, var(--dark-color), rgba(145, 233, 255, 0.2)), repeating-linear-gradient(220deg, rgb(0, 0, 0) 0px, rgb(0, 0, 0) 19px, transparent 19px, transparent 22px), repeating-linear-gradient(189deg, rgb(0, 0, 0) 0px, rgb(0, 0, 0) 19px, transparent 19px, transparent 22px), repeating-linear-gradient(148deg, rgb(0, 0, 0) 0px, rgb(0, 0, 0) 19px, transparent 19px, transparent 22px), linear-gradient(90deg, rgb(255, 255, 250), rgb(240, 240, 240));
}

.title {
  position: absolute;
  top: 0;
  left: 0;
  color: white;
  font-family: 'Courier New', Courier, monospace;

  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-content: center;
  align-items: center;

  width: 100%;
  height: 100vh;
  text-shadow: 0 0 20px white;
  letter-spacing: 0px;
}

@media (min-width: 500px) {
  .title {
    letter-spacing: 20px;
  }
}

@keyframes typing {
  from {
    opacity: 0;
  }

  to {
    opacity: 1;
  }
}

/* Terapkan animasi dengan delay */
.title span {
  opacity: 0;
  animation: typing 1s ease forwards;
  animation-delay: var(--delay);
}

a {
  text-decoration: none;
}

.btn {
  border: none;
  width: 15em;
  height: 5em;
  border-radius: 3em;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 12px;
  background: #1C1A1C;
  cursor: pointer;
  transition: all 450ms ease-in-out;
}

.sparkle {
  fill: #AAAAAA;
  transition: all 800ms ease;
}

.text {
  font-weight: 600;
  color: #AAAAAA;
  font-size: medium;
}

.btn:hover {
  background: linear-gradient(0deg, #A47CF3, #683FEA);
  box-shadow: inset 0px 1px 0px 0px rgba(255, 255, 255, 0.4),
    inset 0px -4px 0px 0px rgba(0, 0, 0, 0.2),
    0px 0px 0px 4px rgba(255, 255, 255, 0.2),
    0px 0px 180px 0px #9917FF;
  transform: translateY(-2px);
}

.btn:hover .text {
  color: white;
}

.btn:hover .sparkle {
  fill: white;
  transform: scale(1.2);
}
