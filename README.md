## Personal quick-scripting spaces using [Pravdomil's type declarations](https://github.com/pravdomil/types-for-adobe#readme):

![](https://thumbs.gfycat.com/ImpressiveFondGreatargus-size_restricted.gif)

> The above is using a personal fork of renderTom's [Adobe Script Runner](https://github.com/rendertom/VSCode-Adobe-Script-Runner), but I'll make a dedicated typescript extension for VSCode that will have the same functionality (and replace some of these steps automatically).

``` bash
# Clone repository
git clone https://github.com/Inventsable/Adobe-Typescript-Sandbox.git

# Install node dependencies (currently commented out because node_modules is not in .gitignore and will be included in git clone)
# npm install

# Now when using VSCode with no additional plugins/extensions (or Atom or any Editor with Typescript plugins/extensions enabled), typing anything into the app/main.ts files will demonstrate autocomplete and access to the OMV.
```

## If doing a manual setup for your own project:

``` bash
# Create a package.json in the root folder of your project if one doesn't already exist:
npm init -y

# Install the type declarations
npm install pravdomil/types-for-adobe

# Place the corresponding tsconfig.json file into your scripting folder like above.
# For added control, you can explicitly define which .ts files are compiled into which .jsx.
```

## Compile on save will not work unless you hit Ctrl+Shift+B and run a Task to watch the file: `tsc: watch - (relative path to tsconfig.json)`

![](https://thumbs.gfycat.com/NeighboringLivelyLeopard-size_restricted.gif)