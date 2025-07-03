# About the Project

This project focuses on building a solid foundation in **Semantic HTML** while emphasizing **accessibility**, **SEO optimization**, and the implementation of **ARIA roles** for enhanced usability. 

Through incremental tasks, learners will structure and enhance a web page to make it not only visually organized but also optimized for screen readers and search engines. By the end of the project, learners will understand the importance of semantic elements and accessibility features in modern web development.

---

## 🎯 Learning Objectives

- **Master Semantic HTML**  
  Learn to structure web pages using semantic elements such as `<header>`, `<main>`, `<article>`, `<section>`, and `<footer>` for better content organization and accessibility.

- **Optimize for SEO**  
  Understand how to improve the visibility of your webpage through appropriate usage of meta tags and proper document structure.

- **Enhance Accessibility**  
  Implement ARIA roles and attributes to make web forms and content more accessible to users with disabilities.

- **Understand Form Design Best Practices**  
  Learn to create accessible and user-friendly forms using modern HTML techniques.

- **Adopt Incremental Development**  
  Practice progressive enhancement by building upon the foundation of each previous task.

---

## ✅ Requirements

- A working understanding of **HTML5**
- Familiarity with **semantic HTML elements** and their purpose
- Basic knowledge of **SEO** and its importance in web development
- Awareness of **web accessibility standards**, including ARIA roles and attributes


# TASKS

## Task 0
### 0. Creating a Structured HTML Document Using Semantic Elements  

#### Objective  
<p><b>Practice structuring a simple HTML document using semantic elements.</b></p>

#### Instructions  

Create your first HTML file named `0-index.html` with the following structure:

1. Inside the `<html>` tag, create:
   - An empty `<head>` tag  
   - An empty `<body>` tag  

2. Inside the `<body>` tag:
   - Add a `<header>` that contains a `<nav>` with **at least three links**
   - Create a `<main>` section that contains:
     - An `<article>`
       - Inside the article, add:
         - An `<h1>` tag for the **title**
         - A `<section>` for the **content**
   - Add a `<footer>` with copyright information:
     ```
     ©copyright
     ```

---

##### 🔔 Reminder  
The structure of an HTML file **starts with** the `<!DOCTYPE html>` declaration.

---

## Task 1  
### 1. Enhancing HTML Document with Meta Tags and Title for SEO and Accessibility  
**Mandatory**

---

### Objective  
To enhance the structure of the HTML document by adding meta tags for improved SEO, accessibility, and responsiveness, while properly defining the document’s character set and title.

---

### Instructions  

- Copy the content of `0-index.html` into `1-index.html`

- Inside the `<head>` tag, add the following:

  1. A `<meta>` tag with `charset="utf-8"`
  2. Four additional meta tags:
     - `name="description" content="A blog post about semantic HTML and accessibility practices"`
     - `name="keywords" content="HTML, Semantic, Accessibility, Blog, SEO"`
     - `name="author" content=""` *(Fill in with your name or leave blank for now)*
     - `name="viewport" content="width=device-width, initial-scale=1.0"`
  3. A `<title>` tag with the text:  
     ```
     Semantic HTML Blog Post
     ```

---

## Task 2  
### 2. Creating a Blog Post Layout Using Semantic HTML Elements  
**Mandatory**

---

### Objective  
Apply semantic elements to create a blog post layout.

---

### Instructions  

- Copy the content of `1-index.html` into `2-index.html`

- Inside the `<header>` tag:
  - Add an `<h1>` with the content: `My Blog`
  - Add a `<nav>` tag
    - Inside the `<nav>`, add a `<ul>` with **3 `<li>`** elements:
      - Home
      - About
      - Contact

- Inside the `<main>` tag's `<article>`:
  - Add a `<header>` tag with:
    - An `<h2>` tag: `Understanding Semantic HTML`
    - A `<p>` tag:  
      ```
      Published on <time datetime="2024-09-10">September 10</time>
      ```

  - Inside the `<section>` tag:
    - `<h3>` tag: `Introduction`
    - `<p>` tag:  
      ```
      Semantic HTML helps improve the accessibility and SEO of your website. In this post, we’ll explore its benefits and how to implement it.
      ```

  - Below the first section (after closing it), add another `<section>`:
    - `<h3>` tag: `Main Content`
    - `<p>` tag with:
      ```
      Using elements like 
      <code>&lt;article&gt;</code>, 
      <code>&lt;section&gt;</code>, 
      <code>&lt;header&gt;</code> 
      ensures that both users and search engines can better understand the structure and content of a webpage.
      ```
    - `<figure>` with:
      - `<img src="" alt="example">`
      - `<figcaption>`: `An illustration of semantic HTML elements`

  - Add a third `<section>`:
    - `<h3>` tag: `Conclusion`
    - `<p>` tag:  
      ```
      By adopting semantic HTML, you enhance your site's accessibility, improve SEO, and make the content easier to navigate.
      ```

  - Add a `<footer>` inside the `<article>` with:
    - `<p>` tag: `Written by <name>`
    - `<p>` tag: `Published on 2024-09-11`

🛠 *Note: All these changes must be made **inside the `<article>` tag** within `<main>`.*

🧠 *Don’t forget to close each tag!*

---

## Task 3  
### 3. Enhancing Form Accessibility with ARIA Roles and Attributes  
**Mandatory**

---

### Objective  
Implement ARIA roles to improve accessibility in a form.

---

### Instructions  

- Copy the content of `2-index.html` into `3-index.html`

- Inside the `<main>` element, add a new `<section>` containing a `<form>` with the following attributes:
  - `action="#"`  
  - `method="POST"`  
  - `aria-labelledby="form-title"`  
  - `role="form"`

- Inside the `<form>`, add the following:

  1. A `<div>` containing:
     - `<label for="name">Name</label>`
     - `<input type="text" id="name" name="name" aria-required="true">`

  2. A second `<div>` containing:
     - `<label for="email">Email</label>`
     - `<input type="text" id="email" name="email" aria-required="true">`

  3. A third `<div>` containing:
     - `<button type="submit" aria-label="Submit the form">Submit</button>`

  4. A `<div>` with:
     - `aria-live="polite"`
     - `role="alert"`

🧠 *As always, make sure to close each tag properly.*
