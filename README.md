# author-list

Author List
Example:
TweetWorld

An application used to retrieve data form https://github.com/lukePeavey/quotable#list-authors to show a list of author user can mark as their favourite and subsequently remove from favorite list, built with React, React-Router, JavaScript, and CSS.

Example:
This project is currently at its version-1.

Project Screen Shot(s)
Example:

(https://ibb.co/FKvMG8n)
(https://ibb.co/MMZLkns)

Installation and Setup Instructions
Example:
Clone down this repository. You will need node and npm installed globally on your machine.

Installation:

npm install

To Run Test Suite:

npm test

To Start Server:

npm start

To Visit App:

localhost:3000
localhost:3000/favorite

Reflection

This was a weekend project built for a react asessment test. Project goals was to finish the given task in stipulated time with certain features and technologies of react to be used.

One of the main challenges I ran into was Routing. This lead me to spend a few hours on a research spike into how react router changed from v-5 to v-6. I was able to make it work after a little diligent reading.

I designed the app to fetch data on initial component mount and then as user select next or previous page a server side pagination is handled by changing the the url to adapt to current pages state.

Routing is added on root of the components and for different route I simply render the list sent as a prop to that Author component. For home or "/" path author list is always coming from the api. And to render the favorite list component in "/favorite" route, I pass author list from local storage.

I set the local storage everytime a user adds or remove an item from the list which is passed as a referene from parent component(App.js) to its child component(Author.js) which triggers the render. Conditional rendering is used to toggle button text and style.

At the end of the day, the technologies implemented in this project are React, React-Router 6.0 and a significant amount of JSX, and CSS. I chose to use the create-react-app boilerplate to minimize initial setup and invest more time in diving into weird technological rabbit holes.
