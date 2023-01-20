# Create NPM Package
##

**Step No 1:** 
create 2 folders one for the package and the other for testing


**Step No 2:**
Go to the package folder and open it in the terminal to create a `package.json` file without using the -y flag. After completion of the `package.js` file add a new file called `index.js`. 

`index.js` is the entry point file of the package. 
 

**Step No 3:**

Add some basic functions for testing purposes.

```jsx
function isACME(string) {
    return string === 'ACME';
}

module.exports = isACME;
```

after create these two files this is ready to publish.

**Step No 4:**

Test package locally do run below command in the terminal

```jsx
npm link
```

to test locally follow below steps

- to create a `script.js` file in the test folder or any empty folder and write script for testing
```jsx
const isAcme = required('is-acme');

console.log(isACME('ACME');
```

Step 5: 

Publish package 

to publish package follow below command. Before running this command make sure you are logged in on npmjs.com.

```jsx
// to publish package
npm publish

// publish package for public
npm publish --access=public

// publish package for dev depdencies 
npm publish --scope=dev-simplifed

```
