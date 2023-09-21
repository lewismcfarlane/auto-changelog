# auto-changelog
## Tutorial
Clone Repo - git clone (SSH link here)
Setup nodejs package .json along with an entry index file
yarn init -y      and add index.js file
Add the following script to package.json
```
 "scripts": {
    "start": "node index.js",
  },
  ```
yarn start will run the index.js
Commit changes with proper convention "fix/feat: message here"
Install and set up the standard-version as a feature commit: ```
yarn add -D standard-version
```
and add command to run the standard-version to the scripts in package.json
``` "scripts": {
    "start": "node index.js",
    "release": "standard-version"
  },
  ```
commit this change as a feature to the repository

The feature is setup and can be utilised with
```
yarn release
```

and then changes can be pushed to GitHub repository
