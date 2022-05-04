# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Overview

### The challenge

### Links

- [Solution](https://www.frontendmentor.io/solutions/learning-tailwind-6-rk09zeeIq)
- [Live site](https://lyons-frontend-mentor.github.io/stats-preview-card-component/)

### Built with

- HTML
- TailwindCSS

## Reflection

The trickiest part of this design was handling the intermediate states, as there's only an image for desktop and an image for mobile. On tablet-sized screens, the horizontal layout doesn't really work since either:

- The image needs to take up half of the horizontal space, which cramps the text content
- The image needs to take up the remaining horizontal space after the text content, which is so small that the aspect ratio of the image forces the _height_ of the image to be too small.

Thus, I had the mobile layout extend for a relatively large width, until there would be enough room for both the image and the text content in the horizontal layout. Another solution may have been to zoom in on a particular part of the image in to fix the height deficit described in the latter case above, but that would probably look weird as it would crop out a lot of the image, which has important elements (the people) along the edges.

After that, it was a matter of tweaking margins and paddings in the intermediate state to avoid the image being to short for the container, until there was enough screen real estate for everything to breathe.

### Continued development

I'll continue practicing Tailwind on challenges like this. The Newbie challenges on Frontend Mentor are nice since there's usually only one major design challenge to focus on (for me at least), like transitioning the layouts in this case. Soon I'll start the Junior challenges, which will bring multiple concepts together in a single challenge, and so on.
