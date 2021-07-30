---
title: "TypeScript Project Quickstart with test"
excerpt: "Quickly setup TypeScript project for small/personal projects"

categories:
  - practice
tags:
  - [javascript, typescript, test, jest, project, set up]

toc: true
toc_sticky: true
 
date: 2021-07-29
last_modified_at: 2021-07-29
---

## Intro
Our engineering team at Browze, we have great activities related to tech.  
`workshop` is one of them and has twice a week.

Usually, the workshop is lead by an engineer manager.
He gives us a problem such as Bowling game, Mars Rover and Game of Life.
We divide into two teams to solve this problem; discuss TDD, pair programming.

To build a solution program, quick setup skills give more time to discuss problems and code.

My colleague [Luis](https://github.com/luisrudge) shared his knowledge and I am writing it based on what he taught.


## Practice

### <u>1. Install</u>
**ts-jest**: To use Jest to test projects written in TypeScript.
```bash
yarn init -y
yarn add -D @types/jest jest typescript ts-jest
```
Creating ts-jest config
```bash
yarn ts-jest config:init
```

### <u>2. Add script</u>
Add script `test` in **package.json**
```json
  "scripts": {
    "test": "jest --watchAll"
  }
```
It will look like this.
```json
{
  "name": "setup",
  "version": "1.0.0",
  "main": "index.js",
  "license": "MIT",
  "devDependencies": {
    "@types/jest": "^26.0.24",
    "jest": "^27.0.6",
    "ts-jest": "^27.0.4",
    "typescript": "^4.3.5"
  },
  "scripts": {
    "test": "jest --watchAll"
  }
}
```

### <u>3. Create my first fake test</u>
Create new file:`teset.spec.ts` in root
Add first test
```js
describe('my test', () => {
  it("works!", () => {
    expect(1).toBe(1);
  })
})
```
![first-fake-test-file](https://user-images.githubusercontent.com/45175926/127593316-d05c1d55-0a5b-4eed-ab8f-07d57921251c.png)

### <u>4.Run test</u>
run test command
```bash
yarn test
```
![fake-test-result](https://user-images.githubusercontent.com/45175926/127593999-92ee804d-80ba-4b52-b05e-2c061dfc3c59.png)

### <u>5.Create `Account.ts` file</u>
To check if test is working well with ts code in root.
  - Create new file `Account.ts`
  - export `Account` class
  - create `works()` method with return `true`
  
```js
export class Account {
  works() {
    return true;
  }
}
```

### <u>6. Test `works()` method</u>
Change test in `test.spec.ts`
```js
expect(new Account().works()).toBe(true);
```
`test.spec.ts` should look like this.

```js
import { Account } from './Account';

describe('my test', () => {
  it("works!", () => {
    expect(new Account().works()).toBe(true);
  })
})
```

### <u>7. Run</u>
Create `runthis.ts`
```js
import { Account } from './Account';

console.log(new Account().works());
```
**ts-node**: To execute TypeScript files or run TypeScript in a REPL environment.
```bash
yarn add -D ts-node
```
run
```bash
npx ts-node runthis.ts
```
