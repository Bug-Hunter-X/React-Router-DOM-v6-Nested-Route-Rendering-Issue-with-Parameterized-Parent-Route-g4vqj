# React Router DOM v6 Nested Route Rendering Issue

This repository demonstrates a bug in React Router DOM v6 where nested routes fail to render correctly when a parent route includes URL parameters.  The issue is specifically related to the interaction between routes with and without parameters.

## Description

The `User` component, which is intended to render nested routes, does not display correctly.  This occurs despite the `Home` and `About` components rendering as expected. The root cause seems to be the presence of the parameterized `path="/users/:userId"` route.

## Setup

1. Clone the repository.
2. Install dependencies: `npm install`
3. Run the application: `npm start`

## Solution

The solution involves using the `useParams` hook correctly within the nested route component. The solution file demonstrates how this solves the issue and properly renders the nested routes.