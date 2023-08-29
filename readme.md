[![License](https://img.shields.io/badge/license-no-red.svg)]()
# TypeScript and JavaScript Module Example

This is a simple example project that demonstrates how to create a module with TypeScript and use it in both TypeScript and JavaScript files.

## create a file
This file includes typescript logic. Make sure to declare exports.

send.ts:
```typescript
export const send = () => {
    return 'hello world!'
}
```
## cli commands
```bash
tsc --init
```
Initialized typescript and creates tsconfig.json in your project.
```bash
tsc send.ts
```
Creates only javascript supported version from your script. You can excucute this command and see a new file being created or follow next wich creates that same file (if not exists) and another file with the declarations.
```bash
tsc send.ts --declaration
```
This generates the JavaScript implementation file (send.js) and the corresponding TypeScript declaration file (send.d.ts).

## run & test
```bash
node app.js
```
node commands runs for javascript files, if no other file has the same name with other extention, then you can run "node app", it will work.
```bash
ts-node test.app.ts
```
ts-node command runs typescript files, same with node, you can run "ts-node test.app" when no other same name was used.
## installations
- install recommended node or if using previous version install that one here: https://nodejs.org/en
- use tsc and typescript globally on your computer by using command in bash or powershell and use **npm install -g typescript**
- install ts-node globally on your computer: **npm install -g ts-node**, also be found here: https://typestrong.org/ts-node/docs/installation/
## license
There's no copyright or license or other needed for a simple project, created in 15 minutes (with research)