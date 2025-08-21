# Decision Roulette 🎡

Decision Roulette is a simple, yet engaging, single-page web application that helps you make a choice by spinning a colorful wheel. It's built with pure HTML, CSS, and JavaScript, demonstrating a clean and interactive user experience.

## Features

* **Interactive Roulette Wheel:** A visually appealing and animated wheel that spins to a random outcome.

* **Weighted Chances:** The chances of landing on a particular option change with each spin. The chosen option's probability is reduced by 50%, while the probabilities of the other options are increased, making it less likely to get the same result twice.

* **Persistent State:** Uses `localStorage` to save the current probabilities, so your progress is saved even if you close the page and come back later.

* **Reset Option:** A **Reset Chances** button allows you to restore all options to their initial equal probabilities.

* **Responsive Design:** The application is designed to work well on both desktop and mobile devices.

## How It Works

The application uses **JavaScript** to handle the core logic:

1. An array of objects stores the options, their colors, and their current `weight` (probability).

2. When the **Spin!** button is clicked, a random number is generated and compared against the options' weights to determine a winner.

3. The wheel is then rotated with a CSS `transform` to land on the winning option, providing a smooth animation.

4. After the spin, the winning option's weight is reduced by 50%, and the remaining percentage is redistributed among the other options.

5. The new, adjusted weights are saved to `localStorage`, ensuring the changes are persistent.

6. The **Reset Chances** button clears the saved data from `localStorage` and restores the original weights.

## Getting Started

To run this project, simply download the `index.html` file and open it in any modern web browser. No server or build tools are required.

## Contributing

The main issue with the labels has been resolved, but there's always room for improvement! If you'd like to contribute, pull requests for new features, design enhancements, or code improvements are welcome.
