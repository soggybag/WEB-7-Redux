# Passwords Project

This project will be built in React or React Native. The premise of the project 
is a utility that generates passwords and stores them. 

- Generate a random password using several methods.
- Save a list of passwords with some notes. 
- Edit and Delete passwords that have been created.

## Discussion

The discussion of this project will include more than just the technical aspects of the project.

- What makes a safe password? 
- What different types of passwords can be generated?
- Is this a viable product? 
  - What are the risks and security issues? 
  - How does JS and the browser as a platform affect this product? 
  
## Technical Discussion 

- What does the project need to display?
- What's the best way to display these things? 
- What views will you need? 
- What should be a component? 
- What about Redux, how should the store be structured? 

## Notes 

For security reasons this project would proabably be best implemented with React Native.

This project will work with `localStorage`. Data and functionality will be encompassed within 
the app, there is no network component. 

### Strategies 

This project will need to save information locally. JavaScript provides `localStorage` as a 
solution. React Native has a native implementation of `localStorage`.

The project will need to navigate across multiple pages. For this you can use React Router. 

Application data needs to be reflected and shared across all pages of the app. For this you can 
use Redux. 

Application data managed by Redux will need to be backed and synched with localStorage. There
are several solutions. The example uses: https://www.npmjs.com/package/redux-localstorage-simple




