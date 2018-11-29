# Learn Redux

Hey there, and welcome to the repo for Reduxstagram! In here, you'll see a single page application I made, in attempt to understand how to integrate Redux with React. I'm not going to say it's an _instagram clone_, but ya know. The finished product can be demoed online at [reduxstagram.leander.xyz](reduxstagram.leander.xyz).

## Using the app

You can use this app just like you would any photo-sharing app. Upon load, you'll be greeted with a bunch of random photos with some captions, likes, and comments. You can scroll through and click on any photo you like to see more details.

Upon click, you'll be routed to the detailed photo view, where the picture will be enlarged, alone with the option to _add_ or _delete_ any comments there. You can also like the photos from either view, at any time.

If you click on the logo, you'll be taken back to the base page, where your changes will still be saved, until page reload!

## How it works

This app was actually bootstrapped a long time ago, so it doesn't use `create-react-app`. Either way, to run it, simply use the command `npm run dev`.

The app itself is only uses a single `store`, with one `Provider` component, passing along to a `connect`ed _App_ component. In Redux' global state, the comments, likes, captions, and authors are stored for every post. 

As for the URL, `react-router` is used in tandom with redux to allow for page-changing to log the `PAGE_CHANGE` action. It can also be tracked via the [Redux DevTools](https://chrome.google.com/webstore/detail/redux-devtools/lmhkpmbekcpmknklioeibfkpmmfibljd?hl=en)!

## Creds

I was able to create this application through the help of a course, developed by [Wes Bos](wesbos.com) entitled [Learn Redux](learnredux.com). If you've stumbled upon this repo, in attempt to learn Redux, I highly recommend his courses and wish you the best of luck!
