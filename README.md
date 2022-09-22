---
```shell
    Error: Could not find module with name: @electron-forge/maker-squirrel
```
# If you are using Windows, this works for me:

Run 
```shell
    npm i electron-winstaller --save-dev --ignore-scripts
```

Install [Z zip](https://www.7-zip.org/download.html) in your computer. 
After installed, 
- go to C:\Program Files (x86)\7-Zip
- and copy both 7z.dll and 7z.exe files to /path/to/your_project/node_modules/electron-winstaller/vendor 
- if they are not still there.

Run  again

```shell 
    npx electron-forge import
```

Then try run npm run make again. I hope it works.

PS. [Found in git discussion](https://github.com/electron-userland/electron-forge/issues/2656)
---