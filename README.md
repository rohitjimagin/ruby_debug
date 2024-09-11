# Using Debugger in VSCode for Ruby

Follow these steps to set up and use the Ruby debugger in VSCode:

## 1. Install the Debug Gem
Add the following line to your `Gemfile`:
```ruby
gem 'debug'
```
Then run: 
```bash
bundle install
```

### 2. Install the Debugger Extension in VSCode
Install the [VSCode rdbg Ruby Debugger](https://marketplace.visualstudio.com/items?itemName=KoichiSasada.vscode-rdbg) from the marketplace.

### 3. Add Breakpoints
Place breakpoints in the desired file within your Ruby code in VSCode.

### 4. Create launch.json File
In your project, create a .vscode folder (if it doesn't exist already) and add a launch.json file with the following content:

```json
{
  "version": "0.2.0",
  "configurations": [
    {
      "type": "rdbg",
      "name": "Attach with rdbg",
      "request": "attach"
    }
  ]
}
```

### 5. Video Reference

<!-- add video from ./videos/debug.mov -->

![Debugging in VSCode](./videos/debug.mov)

