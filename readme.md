# 

Running `npm run lint` produces the following error:

    > @kasparsd/wp-scripts-eslint-prettier-bug@1.0.0 lint /Users/kaspars/Projects/wp-scripts-eslint-prettier-bug
    > eslint ./src

    Error: Cannot find module 'prettier'
    Occurred while linting /Users/kaspars/Projects/wp-scripts-eslint-prettier-bug/src/script.js:1
        at Function.Module._resolveFilename (module.js:548:15)
        at Function.Module._load (module.js:475:25)
        at Module.require (module.js:597:17)
        at require (/Users/kaspars/Projects/wp-scripts-eslint-prettier-bug/node_modules/v8-compile-cache/v8-compile-cache.js:161:20)
        at Program (/Users/kaspars/Projects/wp-scripts-eslint-prettier-bug/node_modules/eslint-plugin-prettier/eslint-plugin-prettier.js:162:26)
        at listeners.(anonymous function).forEach.listener (/Users/kaspars/Projects/wp-scripts-eslint-prettier-bug/node_modules/eslint/lib/linter/safe-emitter.js:45:58)
        at Array.forEach (<anonymous>)
        at Object.emit (/Users/kaspars/Projects/wp-scripts-eslint-prettier-bug/node_modules/eslint/lib/linter/safe-emitter.js:45:38)
        at NodeEventGenerator.applySelector (/Users/kaspars/Projects/wp-scripts-eslint-prettier-bug/node_modules/eslint/lib/linter/node-event-generator.js:254:26)
        at NodeEventGenerator.applySelectors (/Users/kaspars/Projects/wp-scripts-eslint-prettier-bug/node_modules/eslint/lib/linter/node-event-generator.js:283:22)
    npm ERR! code ELIFECYCLE
    npm ERR! errno 2
    npm ERR! @kasparsd/wp-scripts-eslint-prettier-bug@1.0.0 lint: `eslint ./src`
    npm ERR! Exit status 2
    npm ERR! 
    npm ERR! Failed at the @kasparsd/wp-scripts-eslint-prettier-bug@1.0.0 lint script.
    npm ERR! This is probably not a problem with npm. There is likely additional logging output above.

    npm ERR! A complete log of this run can be found in:
    npm ERR!     /Users/kaspars/.npm/_logs/2020-02-04T10_54_35_609Z-debug.log

And the output of `2020-02-04T10_54_35_609Z-debug.log` is:

    0 info it worked if it ends with ok
    1 verbose cli [ '/usr/local/Cellar/node@8/8.17.0/bin/node',
    1 verbose cli   '/usr/local/bin/npm',
    1 verbose cli   'run',
    1 verbose cli   'lint' ]
    2 info using npm@6.13.6
    3 info using node@v8.17.0
    4 verbose run-script [ 'prelint', 'lint', 'postlint' ]
    5 info lifecycle @kasparsd/wp-scripts-eslint-prettier-bug@1.0.0~prelint: @kasparsd/wp-scripts-eslint-prettier-bug@1.0.0
    6 info lifecycle @kasparsd/wp-scripts-eslint-prettier-bug@1.0.0~lint: @kasparsd/wp-scripts-eslint-prettier-bug@1.0.0
    7 verbose lifecycle @kasparsd/wp-scripts-eslint-prettier-bug@1.0.0~lint: unsafe-perm in lifecycle true
    8 verbose lifecycle @kasparsd/wp-scripts-eslint-prettier-bug@1.0.0~lint: PATH: /usr/local/lib/node_modules/npm/node_modules/npm-lifecycle/node-gyp-bin:/Users/kaspars/Projects/wp-scripts-eslint-prettier-bug/node_modules/.bin:/usr/local/lib/ruby/gems/2.6.0/bin:/usr/local/opt/php@7.0/bin:./vendor/bin:/Users/kaspars/.composer/vendor/bin:/usr/local/sbin:/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin
    9 verbose lifecycle @kasparsd/wp-scripts-eslint-prettier-bug@1.0.0~lint: CWD: /Users/kaspars/Projects/wp-scripts-eslint-prettier-bug
    10 silly lifecycle @kasparsd/wp-scripts-eslint-prettier-bug@1.0.0~lint: Args: [ '-c', 'eslint ./src' ]
    11 silly lifecycle @kasparsd/wp-scripts-eslint-prettier-bug@1.0.0~lint: Returned: code: 2  signal: null
    12 info lifecycle @kasparsd/wp-scripts-eslint-prettier-bug@1.0.0~lint: Failed to exec lint script
    13 verbose stack Error: @kasparsd/wp-scripts-eslint-prettier-bug@1.0.0 lint: `eslint ./src`
    13 verbose stack Exit status 2
    13 verbose stack     at EventEmitter.<anonymous> (/usr/local/lib/node_modules/npm/node_modules/npm-lifecycle/index.js:332:16)
    13 verbose stack     at emitTwo (events.js:126:13)
    13 verbose stack     at EventEmitter.emit (events.js:214:7)
    13 verbose stack     at ChildProcess.<anonymous> (/usr/local/lib/node_modules/npm/node_modules/npm-lifecycle/lib/spawn.js:55:14)
    13 verbose stack     at emitTwo (events.js:126:13)
    13 verbose stack     at ChildProcess.emit (events.js:214:7)
    13 verbose stack     at maybeClose (internal/child_process.js:915:16)
    13 verbose stack     at Process.ChildProcess._handle.onexit (internal/child_process.js:209:5)
    14 verbose pkgid @kasparsd/wp-scripts-eslint-prettier-bug@1.0.0
    15 verbose cwd /Users/kaspars/Projects/wp-scripts-eslint-prettier-bug
    16 verbose Darwin 19.3.0
    17 verbose argv "/usr/local/Cellar/node@8/8.17.0/bin/node" "/usr/local/bin/npm" "run" "lint"
    18 verbose node v8.17.0
    19 verbose npm  v6.13.6
    20 error code ELIFECYCLE
    21 error errno 2
    22 error @kasparsd/wp-scripts-eslint-prettier-bug@1.0.0 lint: `eslint ./src`
    22 error Exit status 2
    23 error Failed at the @kasparsd/wp-scripts-eslint-prettier-bug@1.0.0 lint script.
    23 error This is probably not a problem with npm. There is likely additional logging output above.
    24 verbose exit [ 2, true ]