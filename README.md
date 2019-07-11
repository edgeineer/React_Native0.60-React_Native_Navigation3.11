# React_Native0.60-React_Native_Navigation3.11

To use react-native-navigation 3.11 in react-native 0.60.2 

  npm install react-navigation
  npm install react-native-gesture-handler
  react-native link react-native-gesture-handler
  
  Add following in new file - react-native.config.js
  
  module.exports = {
    dependencies: {
      'react-native-gesture-handler': {
        platforms: {
          android: null,
          ios: null,
        },
      },
    },
  };
  
  Add following in package.json
  
  "scripts": {
    "postinstall": "jetify"
  }
  
  npm install jetifier
  npx jetify
  npx react-native run-android
  react-native run-android