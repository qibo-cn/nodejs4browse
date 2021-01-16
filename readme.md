## require nodejs package in \<script\> in html, such as 'uniq'

### install nodejs, browserify

```shell
npm install -g browserify
```

### make directory: nodejs4browse, and initial nodejs project

```shell
mkdir nodejs4browse
npm init
npm install --save uniq
```

### create index.js, index.html, browse.js

```shell
touch index.js index.html browse.js
```

### package files

```shell
browserify -r uniq index.js > bundle.js
```

### require uniq in \<script\>

```javascript
var uniq = require("uniq");
```

### run index.html in chrome

## refe: https://blog.csdn.net/w88193363/article/details/86238624
