packages to install

eslint (
    - [x] configs:  ESLint Prettier, AirBnb
    plugins:  prettier
    .eslintrc (use https://raw.github.ibm.com/cio-london-xp-farm/Build-Tower/GroupA/.eslintrc.js?token=AAAE67UEH543BJR4HU4G6WTBRZERO)
    .eslintignore

    // run `./node_modules/.bin/eslint --init` 
        ✔ How would you like to use ESLint? · style
    ✔ What type of modules does your project use? · commonjs
    ✔ Which framework does your project use? · none
    ✔ Does your project use TypeScript? · No / Yes
    ✔ Where does your code run? · browser
    ✔ How would you like to define a style for your project? · guide
    ✔ Which style guide do you want to follow? · airbnb
    ✔ What format do you want your config file to be in? · JavaScript
    Checking peerDependencies of eslint-config-airbnb-base@latest
    The config that you've selected requires the following dependencies:

    eslint-config-airbnb-base@latest eslint@^5.16.0 || ^6.8.0 || ^7.2.0 eslint-plugin-import@^2.22.1
    ✔ Would you like to install them now with npm? · No / Yes

)
prettier (
    ✅- [ ] .prettierrc (https://raw.github.ibm.com/cio-london-xp-farm/Build-Tower/GroupA/.prettierrc?token=AAAE67TCQOFJ7QIDBELJB6DBRZFFU)
    ✅- [ ] .prettierignore
)
✅jest (
    ✅ --npm install --save-dev jest
    ✅ config
    ✅ command for watch mode ("test:watch": "jest --watchAll --verbose",)

)
husky(
    stages (?)
    ✅commitmessage
        commitmessage
    ✅-precommit, 
    prepush hooks
)
✅commitlint(
    commitlint config
)
✅typesync
git(
    .gitignore (use https://github.com/github/gitignore/blob/master/Node.gitignore)
)

automatically get eslint to fix.  
    precommit, 
    ✅-lint-staged? 
        gearoid's lint staged:  
            "lint-staged": {
                "*": [
                "npm run detect-secrets"
                ],
                "*.js": [
                "eslint --cache --fix",
                "git add"
                ],
                "**/*.{css,html,js,json,md,page,xml,yaml,yml}": [
                "prettier --write",
                "git add"
                ],
                "package.json": [
                "typesync --silent",
                "sort-package-json",
                "git add"
                ]
          },


set up git repository


