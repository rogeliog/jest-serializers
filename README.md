## This is a WIP - And it is not ready to be used :)

# jest-serializers

A collection of Jest serializers.

## Motivation

Jest's snapshot testing is awesome, but it is currently associated with testing React components. The infrastructure that Jest provides for snapshots is agnostic of React and can be used for a lot of amazing things. I would love to explore what snapshot testing can be used for and provide a way for the community to use this serializers.

Here are some serializers that I think would be interesting things to explore:
* png: A serializer for dealing with images(for example banner.png). Imagine if everytime that a static asset changes a snapshot will be generated and you could get a visual diff of it. This is also particularly useful if you app deals with image processing for example, `grayscale(blur(image))`, would save the processed image in a snapshot. I don't think that this could be done currently with what Jest provides out of the box but we can always contribute back to Jest so support a more robust API for serializers :smile:
* cycle: Allow snapshot tests to work with [Cycle.js](https://cycle.js.org)
* vue: Allow snapshot tests to work with [Vue.js](https://vuejs.org)
* mustache: Allow snapshot tests to work with [Mustache](https://github.com/janl/mustache.js) templates.



## Usage 

```
npm install --save-dev jest-serializers
```

More about Jest's snapshotSerializer config [here](http://facebook.github.io/jest/docs/configuration.html#snapshotserializers-array-string).

### Available serializers

#### `jest-serializers/enzyme`

A snapshot serializer for Jest+Enzyme.

```json
"jest": {
  "snapshotSerializers": ["<rootDir>/node_modules/jest-serializers/enzyme"]
}
```
