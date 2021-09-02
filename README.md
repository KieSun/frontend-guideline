![juntos-somos-devs](https://user-images.githubusercontent.com/3603793/131751022-fda4146c-9ada-4ad0-82fc-d8f0a73acd3f.png)

# Front-end - Guidelines

[![GitHub contributors](https://img.shields.io/github/contributors/juntossomosmais/frontend-guideline.svg)](https://github.com/juntossomosmais/frontend-guideline/graphs/contributors)

> "Every line of code should appear to be written by a single person, no matter the number of contributors." - Chinese Proverb.

The following document describes generic rules of writing in development languages that we use on our Front-end projects, that HTML, CSS, JavaScript, React, and Vue

The idea of this repository is not to be a complete guideline, the target is just to help developers who participate in our projects to be able to inform the coding standards used.

As this is a live document, some rules may not have been applied in old projects and changes can occur at any time.

<a name="summary"></a>

## 📖 Summary

1. [General Code Patterns](#general-patterns)
1.1 [Code Syntax](#code-syntax)
2. [Git](#git)
2.1. [Commit Messages](#commit-messages)
3. [CSS](#css)
3.1. [CSS Code Syntax](#css-syntax)
3.2. [CSS Declaration Order](#css-order)
4. [Javascript](#javascript)
4.1. [Javascript Code Syntax](#javascript-syntax)
    - 4.1.1 [Variables](#variables)

___
   
<a name="general-patterns"></a>

## 1. General Code Patterns

- 1.1. [Code Syntax](#code-syntax) <br>
  
<a name="code-syntax"></a>

### 1.1. Code Syntax

Use soft tabs with two spaces. You need to configure your editor for this.

**✅ Good:**
```js
const obj = {
  prop: "value",
  prop2: "value2",
  prop3: "value3",
}
```

**❌ Bad:**
```js 
const obj = {
    prop: "value",
    prop2: "value2",
    prop3: "value3",
}
```
 
**[⬆ back to summary](#summary)**

---

<a name="git"></a>

## 2. Git

- 2.1. [Commit Messages](#commit-messages) <br>

<a name="commit-messages"></a>

### 2.1. Commit Messages

In order to facilitate the contribution of anyone in a project, all commit messages must be in **English**.

We also use [conventional commit messages](https://www.conventionalcommits.org/en/v1.0.0/), that is, the commit message must be in the form of a sentence, with the first word being an action, and the rest of the sentence a describing text.

**✅ Good:**
```powershell
git commit -m "feat: allow provided config object to extend configs"
git commit -m "docs: correct spelling of CHANGELOG"
git commit -m "feat(lang): add the Portuguese language"
```

**❌ Bad:**
```powershell
git commit -m "Add placeholder on input"
```

**[⬆ back to summary](#summary)**

---

<a name="css"></a>
 
## 3. CSS

- 3.1. [CSS Code Syntax](#css-syntax)
- 3.2. [CSS Declaration Order](#css-order) <br>
  
<a name="css-syntax"></a>

### 3.1. CSS Syntax

Keep one declaration per line.

**✅ Good:**
```css 
.selector-1,
.selector-2,
.selector-3 {
  ...
}
```

**❌ Bad:**
```css
.selector-1, .selector-2, .selector-3 {
  ...
}
```

Separate each ruleset by a blank line.

**✅ Good:**
```css 
.selector-1 {
  ...
}

.selector-2 {
  ...
}
```

**❌ Bad:**
```css
.selector-1 {
  ...
}
.selector-2 {
  ...
}
```

Use lowercase and avoid specifying units is zero-values.

**✅ Good:**
```css
.selector-1 {
  color: #aaaaaa;
  margin: 0;
}
```

**❌ Bad:**
```css
.selector-1 {
  color: #AAAAAA;
  margin: 0px;
}
```

<a name="css-order"></a>

### 3.2. CSS Declaration Order

The declarations should be added in alphabetical order.

**✅ Good:**
```css
.selector {
  background: #fff;
  border: #333 solid 1px;
  color: #333;
  display: flex;
  height: 200px;
  margin: 5px;
  padding: 5px;
  width: 200px;
}
```

**❌ Bad:**
```css
.selector {
  padding: 5px;
  height: 200px;
  background: #fff;
  margin: 5px;
  width: 200px;
  color: #333;
  border: #333 solid 1px;
  display: flex;
}
```

**[⬆ back to summary](#summary)**

<a name="javascript"></a>

## 4. Javascript

- 4.1. [Javascript Code Syntax](#javascript-syntax)
  - 4.1.1. [Variables](#variables) <br>


<a name="javascript-syntax"></a>

### 4.1. Javascript Code Syntax

<a name="variables"></a>

#### 4.1.1 Variables

Use meaningful, pronounceable, and in **English** variable names.

**✅ Good:**
```js
const currentDate = new Date().toLocaleDateString('pt-BR')
```

**❌ Bad:**
```js 
const xpto = new Date().toLocaleDateString('pt-BR')
```

**[⬆ back to summary](#summary)**


---