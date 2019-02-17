# colorconsole - A simple library to add terminal colors to strings.

A simple emojicode library to setup text formatting.

## Install

### Installing directory using yarn

You can use yarn to directory install this project to your packages directory.
```bash
yarn add https://github.com/nathanmentley/emoji-color-console.git --modules-folder packages
```

### (Optional) Setting up a package.json and .yarnrc

You can use a yarnrc and your packages.json file to let yarn manage your emojicode dependancies automatically.

With this method you can a single command to grab all your emojicode dependancies:

```bash
yarn install
```

You'll need to first create a .yarnrc file at the root of your project with this content:

.yarnrc
```
--modules-folder packages
```

Then you'll need to either update or create a package.json file with the dependencies set up like this:

package.json
```json
{
    "name": "emoji-color-console-example",
    "version": "0.0.1",
    "license": "MIT",
    "scripts": {
        "build": "emojicodec ./🔧/🏁.emojic -o bin/app",
        "clean": "rm -f ./🔧/*.o && rm -f ./bin/app",
        "run": "bin/app Example"
    },
    "dependencies": {
        "colorconsole": "https://github.com/nathanmentley/emoji-color-console.git"
    }
}
```

## Example

🔧/🏁.emojic
```emojicode
💭 package imports
📦 colorconsole 👩‍🎨

🏁 ➡️ 🔢 🍇
  😀
    🖌🐇🔶👩‍🎨🖌
      🔤message to style🔤
      🍨
        🆕🔶👩‍🎨🎨💙❗️
        🆕🔶👩‍🎨🎨🤢❗️
        🆕🔶👩‍🎨🎨🌩❗️
        🆕🔶👩‍🎨🎨🌧❗️
        🆕🔶👩‍🎨🎨🌨❗️
        🆕🔶👩‍🎨🎨🌪❗️
      🍆
    ❗️
  ❗️

  ↩️ 0
🍉
```

### Building the library from source.
There is an included package.json with build scripts that should make this pretty easy to build.

In the repo root you should be able to just run:
```bash
yarn run build
```

### Building and running the example project.
There is an included package.json with build scripts that should make this pretty easy to build.

In the repo root you should be able to just run:
```bash
yarn example
```
