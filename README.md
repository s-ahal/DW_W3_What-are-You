# Week 3 - Front End Applications

## How to run the application:

Visit [https://whatareyou2.replit.app/](https://whatareyou2.replit.app/)

## Inspiration/Concept

This is related to a project I was working on surrounding surveillance where I wanted to wear a live body camera that streamed to a webpage. The device was supposed to perform requests to an object detection API and then display the results on the webpage as poetic text.
It's still a work in progress. I built out some of this frontend for another class this week, but wanted to try my hand at using different APIs and manipulating the DOM using the results.

## Process

I used Replit as my development environment. This was pushed to GitHub straight from the Replit interface. The website runs off a Node server using Express. The image the user submits is sent to the backend, where an API request is made to Clarifai's [general image detection model](https://clarifai.com/clarifai/main/models/general-image-detection), then the object results are filtered and sent back to the frontend.
The reason I needed this to happen in the backend is because I didn't want my PAT visible in the frontend code. I wanted the frontend to be simple and to emulate the look of a command line interface. Everything occupies a central column on the page. I reused design elements from [previous](https://sillylittlephone.replit.app/) [projects](https://selectyrpet.replit.app/), so I skipped over the sketching bit.
Getting the API call to work was where I spent most of my time. I had encoding issues with the images and am still wrapping my head around JSON and HTTP request syntax.
