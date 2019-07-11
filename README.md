# React_Native0.60-React_Native_Navigation3.11

This is a boiler plate code for RN-0.60.2 with RNN-3.11

To start
    1. git clone https://github.com/edgeineer/React_Native0.60-React_Native_Navigation3.11.git
    2. npm install
    3. react-native start
    4. react-native run-android
    
Follow below steps in order to install RNN in your own project 
--------------------------------------------------------------
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
  
  
  