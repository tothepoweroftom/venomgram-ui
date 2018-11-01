# venomgram-ui
Reactive UI built with Vue (with Vue-Router and Vuex), transpiled with Babel, and bundled with Webpack. A painless process with Vue CLI 3. Serves as the front-end for [Venomgram](https://venomgram.netlify.com), an Instagram clone built with full-stack JavaScript. The server is a REST API built with Node/Express/MongoDB, check that out [here](https://github.com/ibrahimpg/venomgram-server).

# Layout

**Home icon** - your feed. Displays posts made by people you follow in reverse chronological order.

**Magnifying glass icon** - explore page. Displays all posts made by people you don't follow and don't have blocked.

**Camera icon** - upload page. Select an image, give it a caption, and hit 'Submit' to post it.

**User icon** - your profile page. Update your display picture and bio, handle your account settings, and view pictures you have posted.

# Instructions

In the command line:

`git clone https://github.com/ibrahimpg/venomgram-ui.git`

`cd venomgram-ui`

`npm install`

`npm run build`

Grab the newly created 'dist' folder in your directory and throw it up on Netlify/cPanel/Github Pages or whatever else you use.

# To-do

* Log user out when a fetch response comes back as 'Authentication failed.'

* Create view for looking at another user's profile upon clicking their name in feed/explore.

* Add DM button to the top right of the header (not on the login/registration screen though). Add placeholder UI giving estimate of when this feature will actually be ready.

* Client-side form 'validation' before actual validation. Right now having an empty field goes through to the server which sends back a failed response. Waste of resources.

* A lot of 'i' elements that run the same standard fetch request. Maybe turn it into a component with an 'icon' attribute that is filled with the icon's Font Awesome class.

* Move Heroku and Cloudinary URLs to environmental variables.

* Add 10vh margin to top (and bottom?) of image view modal.