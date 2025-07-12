# Sass & SCSS 

This project focuses on the basics of Sass (Syntactically Awesome Stylesheets), including installation, variables, nesting, and mixins.

---

## 📦 0. Project Set Up

**Objective:** Install and set up SASS

### 🛠 Instructions:
1. Inside the `alx-intermediate-frontend` repository, create a new directory:
```

mkdir 0x03-sass\_scss

````

2. **Linux Installation (Optional):**
```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
exit
# Reopen your terminal
````

3. **Install SASS (Anywhere using Node):**

   ```bash
   npm install sass -v 3.7.4
   ```

4. **Create a File**:

   * `0-installation-script`: Write down the steps you took to install Sass.

**Repo:**

* GitHub repository: `alx-intermediate-frontend`
* Directory: `0x03-sass_scss`
* File: `0-installation-script`

---

## 🧪 1. Debug Output: Hello World

**Instruction:**

* Write a Sass file that prints `Hello world` using `@debug`.

### ✅ Example:

```scss
@debug "Hello world";
```

**Expected Output:**

```bash
0-debug_log.scss:2 DEBUG: Hello world
```

**Repo:**

* File: `0-debug_log.scss`

---

## 🎨 2. Using Sass Variables to Assign Text Color

**Objective:** Use a Sass variable to color HTML tags.

**Instructions:**

* Assign `#3D3D3D` to `body` and `p` tags using a variable.

### ✅ Example:

```scss
$main_color: #3D3D3D;

body {
  color: $main_color;
}

p {
  color: $main_color;
}
```

**Repo:**

* File: `1-color_variable.scss`

---

## 🌿 3. Nesting Selectors

**Instructions:**

* No margin or padding in `body`
* Margin `10px` to `p` tags **inside** `body`
* Must use **nested declarations**

### ✅ Example:

```scss
body {
  margin: 0;
  padding: 0;

  p {
    margin: 10px;
  }
}
```

**Repo:**

* File: `2-nested_tag.scss`

---

## 🧩 4. Margin Mixins

**Instructions:**

* Use a **mixin** to apply:

  * `margin-left` and `margin-right` of `10px` to `body`
  * `margin-left` and `margin-right` of `15px` to `div`

### ✅ Example:

```scss
@mixin set-margins($left, $right) {
  margin-left: $left;
  margin-right: $right;
}

body {
  @include set-margins(10px, 10px);
}

div {
  @include set-margins(15px, 15px);
}
```

**Repo:**

* File: `3-mixin_margins.scss`

---

## ✅ Summary

This project covers:

* Installing Sass
* Writing debug outputs
* Using variables
* Writing nested rules
* Creating and using mixins

All tasks should be inside the `0x03-sass_scss` directory in your `alx-intermediate-frontend` repo.

```


