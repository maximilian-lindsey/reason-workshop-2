# reason-workshop-2

Feedback Form Link: https://docs.google.com/forms/d/e/1FAIpQLSduti27Gold0T3WDtSe04Hi3V-yaBG0ChqAbS-t3-qoe4qsbA/viewform

GraphQL & Reason talk https://www.youtube.com/watch?v=tUIvl2pe8CQ

[Ken Wheeler - ReasonML is Serious Business](https://www.youtube.com/watch?v=lzEweA7RPi0)

## 1. Data structures

Create a data-structure for a chess figure with the following attributes: color, position, kind

- The color can be either black / white
- The position has 2 dimensions on a typical chess board
- The kind describes the value of the figure (king, tower, pawn …)

Put your data-structures in action by storing 2 chess figures in a collection called figures:

- Figure 1: Black, King, on position A1
- Figure 2: White, Tower, on position C7

I recommend to use the playground for this example: https://reasonml.github.io/en/try

Alternative playground: https://sketch.sh/

Tip: You may use lists, arrays, tuples, variants for these tasks

## 2. Data structures II

Create a file Data.re and inside create a list of places with the following properties

- id (generate uuids via https://www.uuidgenerator.net/)
- name
- description
- image containing an url, attribution and attributionUrl (optional)
- address
- phone (optional)
- email (optional)
- coordinates containing lat and lng

## 3. Manipulate Data

1. Create an Array of names based on the places data structure. Print out the array for verification.

Try it without and then use fast-pipe for this task.

2. Pro lesson: create a search funtion. You can give it a string and it will find items based on the place name. For an empty string it returns all entries. Note: There is String and Js.String when using BuckleScript

## 4. ReasonReact

1. Setup the editor -> https://reasonml.github.io/docs/en/editor-plugins
2. Create a new ReasonReact BuckleScript project -> https://reasonml.github.io/reason-react/docs/en/installation

```
npm install -g bs-platform
bsb -init my-react-app -theme react
cd my-react-app && npm install && npm start
# in another tab
npm run webpack
# in another tab
npm run server
```

3. Add your Data.re file
4. Render a list of the place names

## 5. Optional Prop

1. Render the image of each place. Depending on if the attributionUrl is available either render a Link or just the text.

2. Render the phone (which is not always in the list)

3. Pro lesson: Render the description as markdown

Internal note: https://github.com/ReasonVienna/reason-conf/blob/master/src/layouts/util.re

## 6. Styling

1. Style a component using bs-emotion, bs-css or something similar.

## 7. Manage state

1. Allow users to filter the attractions using an input field.

2. Pro lesson: add labels per place and allow to filter by them

Hint: For advanced form management you might like https://github.com/alexfedoseev/re-formality
