# Create new React+Redux app guide

## Step 1 - Create app

```bash
npm install -g create-react-app
create-react-app demo-app
cd demo-app
```
## Step 2 - Install react-router

```bash
yarn add react-router-dom
# or, if you're not using yarn
npm install react-router-dom
```

## Step 3 - Refactor App.js

```js
import React from 'react';
import {
  BrowserRouter as Router,
  Route
} from 'react-router-dom';
// sample component, replace your components here
import {
  Home as HomePage
} from './components/pages';

export default () => {
  return (
    <Router>
      <div>
        <Route exact path="/" component={HomePage}/> // sample component, replace your components here
      </div>
    </Router>
  );
};
```
