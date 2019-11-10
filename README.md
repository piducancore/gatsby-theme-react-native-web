# gatsby-theme-react-native-web

This [theme](https://www.gatsbyjs.org/docs/themes/) adds support for building [Gatsby](https://www.gatsbyjs.org) sites using [React Native](https://github.com/facebook/react-native) components.

## Isn't there a plugin for this already?

Yes, there's one called [`gatsby-plugin-react-native-web`](https://github.com/slorber/gatsby-plugin-react-native-web).

This theme puts that plugin and [its dependencies](https://github.com/slorber/gatsby-plugin-react-native-web/issues/7#issuecomment-472763972) in a single package for _increased <s>lazyness</s> developer experience_:zap:.

## Install

Run the following in your Gatsby site's directory.

```shell
yarn add gatsby-theme-react-native-web
```

## Usage

Once installed, add the theme as a plugin in your `gatsby-config.js`.

```javascript
// gatsby-config.js
module.exports = {
  plugins: [`gatsby-theme-react-native-web`],
}
```

That's it, you can now start building your Gatsby site using React Native components like in the example below.

## Example

```javascript
// src/pages/index.js
import React from "react"
import { StyleSheet, Text, View } from "react-native"

const styles = StyleSheet.create({
  box: { padding: 10 },
  text: { fontWeight: "bold" },
})

export default () => (
  <View style={styles.box}>
    <Text style={styles.text}>Hello, world!</Text>
  </View>
)
```
