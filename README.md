# Solo Desktop

This graphic tool allows easy customization and testing of SoloKeys products and any 3rd party FIDO authenticators.

* MakeCredential and GetAssertion
* Reset
* PIN management
* Firmware update

# WIP

Not yet ready!

# Running

```
cd solo-desktop
npm ci
npx electron-rebuild
npm start
```

# Building a release

Normal users should have an easy to use binary or installer.
To create one, run:

```
npm run release
```

And check the `dist/` folder.  It takes a minute.

# Testing

Tests run in node so you need to rebuild since you're not using electron.

```
npm rebuild
```

Run FIDO client tests.  

```
node main/ctap.js
```


Run FIDO HID tests.  

```
node main/hid.js
```

