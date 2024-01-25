# Hello Arvind CLI 👋

A command-line tool to learn more about me directly in your terminal ;)

<!-- ## What it does 🚀

This CLI script provides a quick overview of Arvind Parekh, including his interests, skills, and relevant links. -->

## How to Run 🏃‍♂️

To run the script, fire up your preferred terminal and use the following command:
(Make sure you have node installed first)

```bash
npx hello-arvind-cli
```

## Screenshots
![Screenshot](https://github.com/ArvindParekh/Hello-Arvind-CLI/assets/71211731/e21b7cc0-38f5-4046-ba82-b23627250161)

## Create your own

Creating your own npx introduction command can be a fun and creative way to share information about yourself. Here's a guide on how to make your own npx introduction command:

- What's npx?
The npx command allows you to run Node.js-based packages without having to globally install them. So you guessed it right, we'll be creating and hosting your own package on the npm registry.


#### Step-1: Create a new project
Start by creating a new project directory for your npx command. Use a meaningful name for your project:

```bash
mkdir npx-intro-command
cd npx-intro-command
```

#### Step 2: Set Up Your Project
Initialize your project with a `package.json file`. You can do this by running:
```bash
npm init -y
```

#### Step 3: Create Your Introduction Script
Create a new file, let's say `index.js`, and write the script that displays your introduction. You can include details such as your name, interests, skills, and links:

```javascript
#!/usr/bin/env node

console.log(`
👋 Hello there! I'm [Your Name].
🚀 [A brief description of yourself and your interests.]
💻 Skills: [List some of your skills or technologies you're familiar with.]

Let's connect:
🌐 GitHub: https://github.com/[YourGitHubUsername]
🐦 Twitter: https://twitter.com/[YourTwitterHandle]
🔗 LinkedIn: https://linkedin.com/in/[YourLinkedInProfile]

Happy coding!
`);
```

#### Step 4: Make It Executable

Make sure your script is executable by running:

```bash
chmod +x index.js
```

Also, include `bin` in your `package.json`:
```json
"bin": {
  "npx-intro-command": "./index.js"
},
```

#### Step 5: Test Locally

- Run `npm link` (A command that allows you to create a symbolic link between a local package and a global installation. This is particularly useful during development when you want to test a package before publishing it.)
- Try running it using `npx package-name`
- If it works, unlink the package using `npm unlink`

#### Step 6: Publish to npm

If everything looks good, you can publish your script to npm. Make sure you have an [npm](https://www.npmjs.com/) account and are logged in:

- Login to npm from your terminal using `npm login`
- Publish your package to registry using the command `npm publish`

And that's it, you're done! I'd love to see the intros you come up with. Feel free to share them on Twitter [@ArvindParekh_21](https://twitter.com/ArvindParekh_21).