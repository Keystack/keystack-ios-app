
# iOS Wrapper for Keytack Cordova application

## Installation

Simple iOS wrapper for Cordova based application.

Used in conjunction with Keystack/keystack-ios-app


After cloning this repository, generate iOS platform files by running:
```sh
cordova add platform ios
```

To install the cordova web application, clone the Keystack/keystack-ios-app from within this repo by running:

```sh
git clone https://github.com/Keystack/keystack-react-app.git
```


After cloning Keystack/keystack-ios-app repository, install dependencies:
```sh
npm install
```
 
From within the keystack-ios-app repository/folder you can compile a build to import into your Cordova wrapper

```sh
npm run build
```

Create a symbolic link to your cordova project folder by running:
```sh
ln -s www/ ../www
```

Once this link has been created, your Wrapper can now be compiled for use in Xcode:
```sh
cd .. [Keystack/keystack-ios-app directory]
cordova build ios
```

## Testing Web applciation with hot reload:

To run the web app and test on your local server using webpack, run:
```sh
npm start
```

The local address will be http://localhost:3011
