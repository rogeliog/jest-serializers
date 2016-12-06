## This is a WIP - And it is not ready to be used :)

# jest-serializers

A collection of jest serializers.

### Motivation

Jest's snapshot testing is awesome, but it is currently associated with testing React components. The infrastructure that jest provides for snapshots is agnostic of React and can be used for a lot of amazing things. I would love to explore what snapshot testing can be used for and provide a way for the community to use this serializers.

```
npm install --save-dev jest-serializers
```

More about Jest's snapshotSerializer config [here](http://facebook.github.io/jest/docs/configuration.html#snapshotserializers-array-string).

## Available serializers

#### `jest-serializers/enzyme`

A snapshot serializer for Jest+Enzyme.

```json
"jest": {
  "snapshotSerializers": ["<rootDir>/node_modules/jest-serializers/enzyme"]
}
```
