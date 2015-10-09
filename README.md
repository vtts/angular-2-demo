# Introduction

A seed project for Angular 2 apps.

It is something similar to the AngularJS Quick Start but does the entire build with gulp.

**Note:** Angular 2.0 is not production ready yet! This seed project is perfect for playing around with the latest versions but do not start new projects with it since a lot of new changes are going to be introduced until the framework is officially released.

# How to start

```bash
git clone https://github.com/erodriguezh/angular-2-demo.git
cd angular2-seed
# If you don't have gulp and/or tsd already installed
npm install -g gulp tsd
npm install
# dev
gulp serve.dev
```

# Directory Structure

```
.
├── app
│   ├── components
│   │   ├── about
│   │   │   ├── about.html
│   │   │   └── about.ts
│   │   │   └── about_spec.ts
│   │   └── home
│   │       ├── home.html
│   │       └── home.ts
│   │       └── home_spec.ts
│   ├── services
│   │       ├── NameList.ts
│   │       └── NameList_spec.ts
│   ├── typings
│   ├── app.css
│   ├── app.html
│   ├── app.ts
│   ├── index.html
│   └── init.ts
├── dist
│   ├── dev
│   └── prod
├── tsd_typings
├── gulpfile.js
├── karma.conf.js
├── package.json
├── test-main.js
├── tsconfig.json
└── tsd.json
```

# Configuration

Default application server configuration

```javascript
var PORT             = 5555;
var LIVE_RELOAD_PORT = 4002;
var APP_BASE         = '/';
```

Configure at runtime

```bash
gulp serve.dev --port 8080 --reload-port 4000 --base /my-app/
```

# Now to extend?

If you want to use your custom libraries:

```bash
npm install my-library --save
vim gulpfile.js
```
Add reference to the installed library in `PATH.src.lib`.

# Running test

```bash
# In a single bash window
gulp test       # or npm test

# Debug - In two bash windows
npm run karma   # 1st window
gulp test-dev   # 2nd window
```

# Change Log

You can follow the [Angular 2 change log here](https://github.com/angular/angular/blob/master/CHANGELOG.md).

# License

MIT
