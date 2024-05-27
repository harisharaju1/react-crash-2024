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
