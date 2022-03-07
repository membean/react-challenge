# Membean React Code Test

## Setup:

To get started you'll need to clone this repository:

```
git clone git@github.com:membean/react-challenge.git
cd react-challenge
```

Install dependencies:

```
yarn
```

To run the app:

```
yarn start
```

To run the tests:

```
yarn test
```

## Objective:

The objective is to make a _(mock)_ API call to get JSON data, which is an array of SVG elements. After stashing that data in Redux, we want you to display the SVGs so that when you hover or click on each SVG, it will render the hex color code as text instead of the the SVG. As a bonus, we'd like you to randomize the color of every SVG so that on each page reload the colors of every React logo changes.

For example, your finished product might look something like the following _(but doesn't have to... don't let use stifle your creativity!)_.

![example](https://github.com/membean/react-challenge/blob/master/example.gif)


## Instructions:

- `fetch()` is mocked on the window. You can use it exactly as you would use `fetch()` normally, except that you do **not** need to call `.json()` on the response. We return the response body by default.
- Look at [/src/api/mockFetch.js](https://github.com/membean/react-challenge/blob/master/src/api/mockFetch.js) to see the JSON data that is returned.

1. Your API call should be made using the provided *Redux API Middleware* file at [/src/store/apiMiddleware.js](https://github.com/membean/react-challenge/blob/master/src/store/apiMiddleware.js).
2. Returned data should be stashed in the Redux store _(obviously)_.
3. Wire up the [App.js](https://github.com/membean/react-challenge/blob/master/src/App.js) component to read data from the Redux store and display the SVGs.
4. Add either a hover or click event to display hex color codes instead of the SVG.

## Testing:

Please stick to using the built in Jest/Enzyme test tools for all your unit tests. We'd like to see the following things tested:

1. Write unit tests for the [apiMiddleware](https://github.com/membean/react-challenge/blob/master/src/tests/apiMiddleware.test.js).
2. Write unit tests for the [rootReducer](https://github.com/membean/react-challenge/blob/master/src/tests/rootReducer.test.js).
3. Write as many unit tests as you think are necessary for the code you write in the [App](https://github.com/membean/react-challenge/blob/master/src/tests/App.test.js) component.

## Submission:

Once you are finished, please push your cloned repo to your Github account _(i.e. https://github.com/YOUR_USERNAME/react-challenge)_ and email the URL to us at [ragav@membean.com](ragav@membean.com).
