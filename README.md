![juntos-somos-devs](https://user-images.githubusercontent.com/3603793/131751022-fda4146c-9ada-4ad0-82fc-d8f0a73acd3f.png)

# Front-end - Guidelines

[![GitHub contributors](https://img.shields.io/github/contributors/juntossomosmais/frontend-guideline.svg)](https://github.com/juntossomosmais/frontend-guideline/graphs/contributors)

> "Every line of code should appear to be written by a single person, no matter the number of contributors." - Chinese Proverb.

The following document describes generic rules of writing in development languages that we use on our Front-end projects, that HTML, CSS, JavaScript, React, and Vue

The idea of this repository is not to be a complete guideline, the target is just to help developers who participate in our projects to be able to inform the coding standards used.

As this is a live document, some rules may not have been applied in old projects and changes can occur at any time.

<a name="summary"></a>

## Summary

<details>
  <summary>General Code Patterns</summary>
  <br/>

  1.1. _[Code Syntax](#code-syntax)_ <br/>
  1.2. _[Variables](#variables)_
  
</details>

<details>
  <summary>Git</summary>
  <br/>

  2.1. _[Commit Messages](#commit-messages)_ <br/>
  
</details>

<a name="general-patterns"></a>

## 1. General Code Patterns

<a name="code-syntax"></a>

### 1.1. Code Syntax

Use soft tabs with two spaces. You need to configure your editor for this.

**❌ Bad:**
```js 
const obj = {
    prop: "value",
    prop2: "value2",
    prop3: "value3",
}
```

**✅ Good:**

```js
const obj = {
  prop: "value",
  prop2: "value2",
  prop3: "value3",
}
```

**[⬆ back to summary](#summary)**

---

<a name="variables"></a>

### 1.2. Variables

Use meaningful, pronounceable, and in **English** variable names.

**❌ Bad:**
```js 
const xpto = moment().format("DD/MM/YYYY")
```

**✅ Good:**

```js
const currentDate = moment().format("DD/MM/YYYY")
```

**[⬆ back to summary](#summary)**
<a name="github"></a>

---
## 2. Git

<a name="commit-messages"></a>

### 2.1. Commit Messages

In order to facilitate the contribution of anyone in a project, all commit messages must be in **English**.

We also use [conventional commit messages](https://www.conventionalcommits.org/en/v1.0.0/), that is, the commit message must be in the form of a sentence, with the first word being an action, and the rest of the sentence a describing text.


**❌ Bad:**
```powershell
git commit -m "Add placeholder on input"
```

**✅ Good:**

```powershell
git commit -m "feat: allow provided config object to extend configs"
git commit -m "docs: correct spelling of CHANGELOG"
git commit -m "feat(lang): add the Portuguese language"
```

**[⬆ back to summary](#summary)**

---