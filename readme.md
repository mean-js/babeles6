Debug ES6 code in Code Visual Studio.

>> npm instlal babel-cli babel-preset-es2015-node6 --save-dev    

>> .babelrc
    "presets": ["es2015-node6"]

>> package.json
    "build": "babel src --out-dir bin --watch --source-maps"
    ** source-maps is important.

>>  launch.json
    "sourceMaps": true,
    "outFiles": ["${workspaceRoot}/bin/**/*.js"]