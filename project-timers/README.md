# WEB 7 Project - Timers 

## Intro

This project will build an app/website that stores a list of timers. Each timer
will run and and stop keeping a cumulative time. This could be used to track 
time spent on freelance or personal projects, used in tracking scientific 
experiments, or any number of uses.

Besides building a project with React and Redux this project will give you a chance to 
take a deeper look at JavaScript concepts like times and dates.

## Decription 

Your project will keep and display a list of timers. It must create new timers and delete 
existing timers. 

Timers will have a name, description, and time. Time represents how long a timer has been 
running. 

The app will show a list of all timers and a detail view of for any single timer. 

Your project needs to meet these criteria: 

- Keeps a list of timers
  - Can add new timers
  - Remove existing timers
  - Time is displayed in a reasonable way
- Timers
  - Keep track of elapsed time for each timer
  - Can be run and paused
  - Have a name/title and short description
- Use Redux to store application state
  - For each timer
    - Time
    - is running or paused
    - Title 
    - Description

## Discussion 

- What is time?
- How is time measured? 
  - What about scale?
    - What is the smallest increment of the time we might want to render? 
    - What is the largest time increment you might render?
- How can time be displayed? 
- How much time might be represented by timers in this app? 
- How does JS handle time?

## Technical Discussion

- What 'views' will this app need? 
  - How would these translate into React components? 
- Starting and stopping timers, how should this be handled? 
  - Can more than one timer be running at the same time? 
- What about persisting data? 
  - Should timers run when the app is closed? 
    - If so how do we track time when the app is not running?

## Notes

This might be good as a native app, might also be good as a web based app. 

For an example of this app turned into a product look at: https://toggl.com

This project in base form is a self contained utility app. Challenges may include moving timer
data to the web where can be shared across multiple devices. 

## Strategies

### Navigation

The app will most likely need to display at least three different views. This will require a 
different approach on the web vs native.

- Web : Use React Router
- Native : React Navigation
  - Or : NavigatorIOS (iOS Only!)

### Application State 

Application state holds the timer data and might displayed in different ways in different views
in your app. The best strategy here is Redux. Redux works equally well with React and 
React Native. 

### Presistent Data

Timer data will be saved locally with app and needs to persist. JavaScript provides `localStorage`. 
This works for web based projects. For native projects you can use AsyncStorage. While React Native 
projects are written in JS they are not running in a web browser consequently `localStorage` is not
available. 

If you are using Redux there are a few 'middleware' helpers that abstract the work of saving 
Application State from Redux. 

- Redux Storage - https://www.npmjs.com/package/redux-storage
  - Note: You'll need to specify the type of store! For native you'll need: reactNativeAsyncStorage

### Working with time

Time is a tricky 



