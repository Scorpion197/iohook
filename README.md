# iohook

## Build for IOS
 - First install `node-gyp` globally
 - clone the repo using `git clone https://github.com/Scorpion197/iohook.git`
 - install the necessary modules using `npm install` 
 - move the `build_def` folder using `cd build_def/darwin` 
 - set up the following `env variables`: 
 ```
 export npm_config_target=22.0.0
 export npm_config_arch=x64
 export npm_config_target_arch=x64
 export npm_config_disturl=https://electronjs.org/headers
 export npm_config_runtime=electron
 export npm_config_build_from_source=true
 HOME=~/.electron-gyp npm install
 ```
 - run the following command: `node-gyp configure` and then `node-gyp build`
