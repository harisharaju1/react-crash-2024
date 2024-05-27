# React + TypeScript + Vite

Vite is similar to create-react-app; it offers out-of-the-box support for React, making it easy to start using Vite with React projects without the need for extensive configuration.

first check-in :
basic React app using Typescript that has a Navbar, Hero section, Job Listings components built using card components name Job Listing

important React concepts:
1. prop drilling - sending information from a prop to another by having props on the componenet being called
2. Tailwind CSS is used to make styling of pages simpler
3. functional components are used, and the plan is to use Hooks for future dev

second check-in :
added routing using react-router-dom

important React concepts:
1. component comms using props
2. component state - using useState
3. events - onClick functionality
4. added react-icons instead of font-awesome so that material UI icons can also be used
    1. npm i react-icons
5. react-router
    1. npm i react-router-dom
    2. all routing in the App.tsx
    3. this pkg is pretty big as this pkg also acts as a base for the Remix SSR framework
    4. *data loaders* in react-router to be dealt with in upcoming commits
    5. import {Route, createBrowserRouter, createRoutesFromElements, RouterProvider} from 'react-router-dom';
    6. *Outlet* + MainLayout
    7. no *a* tags, only *Link* tags
        1. because a tag will do a complete page refresh
        2. whilst Link doesn’t do a actual refresh
    8. add a custom 404 page
  
third check-in :
added json-server to mimic back-end server that returns data

important React concepts:
1. difference between a dependency and a dev dependency
    1. By separating dependencies from dev dependencies, you keep the size of your production-deployed application smaller. This translates to faster loading times and a better user experience. Additionally, it avoids cluttering your production environment with tools only needed for development
2. useEffect allows our React components have a side effect, i.e., bring in something from the outside
3. parameters of a useEffect hook
    1. effect function
    2. dependency array
4. promises, and things to keep in mind when using async/await in TS/JS
    1. Promises provide a way to handle asynchronous operations in a structured and manageable way
    2. they have three states
        1. pending - The initial state, indicating the operation is ongoing
        2. fulfilled - The operation completed successfully, and a value is available
        3.   rejected - The operation failed, and an error reason is available
5. in TS, method parameters are deconstructed as below
const sampleFunction = ({isExample}:{isExample: boolean}) => { ....body of function}

or

const sampleFunction = (props:{isExample: boolean, apiUrl: string}) => { ....body of function}
