# HTML Workshop: Day 1

---

## Table of Contents

1. [Prerequisites & Setup](#1-prerequisites--setup)
2. [Introduction to HTML](#2-introduction-to-html)
3. [HTML Fundamentals](#3-html-fundamentals)
4. [Document Structure](#4-document-structure)
5. [The Head Section](#5-the-head-section)
6. [The Body Section](#6-the-body-section)
7. [Text Content Elements](#7-text-content-elements)
8. [Text Formatting](#8-text-formatting)
9. [Special Elements](#9-special-elements)
10. [Images](#10-images)
11. [Final Project: CV Website](#11-final-project-cv-website)

---

## 1. Prerequisites & Setup

### 1.1 VS Code Installation

Download and install Visual Studio Code from the [official website](https://code.visualstudio.com/).

### 1.2 Required Extensions

Install these extensions in VS Code:

| Extension | Purpose |
|-----------|---------|
| **Prettier** | Code formatter for clean, consistent code |
| **Live Server** | Launch a local server with live reload |
| **Auto Save** | Automatically save your files |

> **Tip:** To install extensions, press `Ctrl + Shift + X` in VS Code and search for the extension name.

---

## 2. Introduction to HTML

**HTML** (HyperText Markup Language) is the standard language used to create the structure of web pages. It consists of a series of **elements** that define different parts of the content, such as headings, paragraphs, images, links, and more.

---

## 3. HTML Fundamentals

### 3.1 HTML Elements

An HTML element is a building block of a web page. It usually consists of:

- **Opening tag:** `<tagname>`
- **Content:** The text or other elements inside
- **Closing tag:** `</tagname>`

**Syntax:**

```html
<tagname>Content goes here</tagname>
```

**Example:**

```html
<p>This is a paragraph.</p>
```

Here `<p>` is the opening tag, `This is a paragraph.` is the content, and `</p>` is the closing tag.

### 3.2 Self-Closing Elements

Some HTML elements do not have any content and are self-closing. They do not require a closing tag.

**Example:**

```html
<img src="image.jpg" alt="Description of image">
<br>
```

### 3.3 Attributes in HTML Tags

Attributes provide additional information about HTML elements and are included within the opening tag. They consist of a **name** and **value** pair, separated by an equals sign.

**Syntax:**

```html
<tagname attribute1="value1" attribute2="value2">Content</tagname>
```

**Examples:**

```html
<link rel="icon" href="path/to/favicon.ico" type="image/x-icon">
```

Here, `rel`, `href`, and `type` are attributes of the `<link>` tag.

```html
<img src="image.jpg" alt="Description of image" width="500" height="600">
```

Here, `src`, `alt`, `width`, and `height` are attributes of the `<img>` tag.

---

## 4. Document Structure

### 4.1 Basic Structure of an HTML Document

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Page Title</title>
  </head>
  <body>
    Main Content Goes Here
  </body>
</html>
```

| Tag | Purpose |
|-----|---------|
| `<!DOCTYPE html>` | Declares the document type |
| `<html>` | Root element of the page |
| `<head>` | Contains metadata (title, favicon, etc.) |
| `<body>` | Contains visible content |

> **VS Code Shortcut:** Type `!` and press `Tab` to auto-generate the basic HTML structure!

---

## 5. The Head Section

The `<head>` section contains metadata about the document.

### 5.1 Setting the Page Title

The `<title>` element sets the title that appears in the browser tab.

```html
<head>
  <title>My First Web Page</title>
</head>
```

### 5.2 Setting a Favicon

The `<link>` element is used to set a favicon (the small icon in the browser tab).

```html
<head>
  <link rel="icon" href="path/to/favicon.ico" type="image/x-icon">
</head>
```

---

### Mini Project 1: Your First HTML Page

**Objective:** Create a simple HTML page with a title and favicon.

**Step-by-Step Instructions:**

1. Create a new file named `project1.html`
2. Type `!` and press `Tab` to generate the basic HTML structure
3. Inside the `<head>` tag:
   - Change the text inside `<title>` tag to `My First Web Page`
   - Add a `<link>` tag with these attributes:
     - `rel="icon"`
     - `href` set to any image URL
     - `type="image/x-icon"`
4. Save the file and open it with Live Server

**Solution:**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>My First Web Page</title>
    <link rel="icon" href="https://upload.wikimedia.org/wikipedia/commons/thumb/0/09/YouTube_full-color_icon_%282017%29.svg/1024px-YouTube_full-color_icon_%282017%29.svg.png" type="image/x-icon" />
  </head>
  <body>
  </body>
</html>
```

---

## 6. The Body Section

The `<body>` section contains all the visible content of your web page. Let's learn what elements we can put inside it.

---

## 7. Text Content Elements

### 7.1 Headings

HTML provides six levels of headings, from `<h1>` (largest) to `<h6>` (smallest).

**Syntax:**

```html
<h1>Main Heading</h1>
<h2>Subheading</h2>
<h3>Sub-subheading</h3>
<h4>Smaller heading</h4>
<h5>Even smaller heading</h5>
<h6>Smallest heading</h6>
```

**Example:**

```html
<!DOCTYPE html>
<html>
<head>
    <title>Heading Examples</title>
</head>
<body>
    <h1>Level 1 Heading - Largest</h1>
    <h2>Level 2 Heading</h2>
    <h3>Level 3 Heading</h3>
    <h4>Level 4 Heading</h4>
    <h5>Level 5 Heading</h5>
    <h6>Level 6 Heading - Smallest</h6>
</body>
</html>
```

### 7.2 Paragraphs

The `<p>` element is used to create paragraphs of text.

**Syntax:**

```html
<p>This is a paragraph.</p>
```

**Example:**

```html
<!DOCTYPE html>
<html>
<head>
    <title>Paragraph Example</title>
</head>
<body>
    <h1>About Nepal</h1>

    <p>
        Nepal is a landlocked country in South Asia. It is located mainly in the
        Himalayas, but also includes parts of the Indo-Gangetic Plain.
    </p>

    <p>
        Nepal has a diverse geography, including fertile plains, subalpine forested
        hills, and eight of the world's ten tallest mountains, including Mount Everest.
    </p>

    <p>
        The capital and largest city is Kathmandu. The official language is Nepali,
        and the currency is the Nepalese Rupee.
    </p>
</body>
</html>
```

### 7.3 Divisions (Containers)

The `<div>` tag is a container that groups other HTML elements together.

**Syntax:**

```html
<div>
    Content and elements go here
</div>
```

**Example:**

```html
<!DOCTYPE html>
<html>
<head>
    <title>Division Example</title>
</head>
<body>
    <div>
        <h2>Student Information</h2>
        <p>Name: Sita Rai</p>
        <p>Roll No: 45</p>
        <p>Class: Bachelor 1st Year</p>
    </div>

    <div>
        <h2>Contact Details</h2>
        <p>Email: sita@example.com</p>
        <p>Phone: 9841234567</p>
    </div>
</body>
</html>
```

---

### Mini Project 2: About Me Page

**Objective:** Create a page about yourself using headings, paragraphs, and divs.

**Step-by-Step Instructions:**

1. Create a new file named `project2.html`
2. Generate the basic HTML structure using `!` + `Tab`
3. Set the page title to `About Me` inside the `<title>` tag
4. Inside the `<body>` tag, add the following in order:
   - Add your name using the `<h1>` tag (main heading)
   - Create the first `<div>` for "About Me" section:
     - Add `About Me` as a subheading using `<h2>` tag
     - Add 2-3 paragraphs about yourself using `<p>` tags
   - Create the second `<div>` for "My Hobbies" section:
     - Add `My Hobbies` as a subheading using `<h2>` tag
     - Add a paragraph listing your hobbies using `<p>` tag

**Solution:**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>About Me</title>
</head>
<body>
    <h1>Ram Sharma</h1>
    
    <div>
        <h2>About Me</h2>
        <p>
            Hello! My name is Ram Sharma. I am a student currently studying 
            Bachelor in Computer Science at Hetauda City College.
        </p>
        <p>
            I am passionate about learning new technologies and building 
            websites. I love solving problems and creating useful applications.
        </p>
    </div>
    
    <div>
        <h2>My Hobbies</h2>
        <p>
            In my free time, I enjoy reading books, playing football, 
            listening to music, and learning to code.
        </p>
    </div>
</body>
</html>
```

---

## 8. Text Formatting

### 8.1 Basic Formatting Tags

| Tag | Purpose | Example |
|-----|---------|---------|
| `<b>` | **Bold** text | `<b>bold text</b>` |
| `<i>` | *Italic* text | `<i>italic text</i>` |
| `<u>` | Underlined text | `<u>underlined text</u>` |

**Example:**

```html
<!DOCTYPE html>
<html>
<head>
    <title>Text Formatting Example</title>
</head>
<body>
    <h1>Text Formatting Examples</h1>

    <p>This is <b>bold</b> text.</p>
    <p>This is <i>italic</i> text.</p>
    <p>This is <u>underlined</u> text.</p>
    <p>This is <b><i><u>bold, italic, and underlined</u></i></b> text.</p>
</body>
</html>
```

### 8.2 Superscript and Subscript

| Tag | Purpose | Example |
|-----|---------|---------|
| `<sup>` | Superscript (above baseline) | X`<sup>`2`</sup>` |
| `<sub>` | Subscript (below baseline) | H`<sub>`2`</sub>`O |

**Syntax:**

```html
<p>This is superscript: X<sup>2</sup></p>
<p>This is subscript: H<sub>2</sub>O</p>
```

> **Practice:**
> - Write H2SO4 using subscript: `H<sub>2</sub>SO<sub>4</sub>`
> - Write E=mc2 using superscript: `E=mc<sup>2</sup>`

---

## 9. Special Elements

### 9.1 Preformatted Text (`<pre>`)

The `<pre>` tag displays text in a fixed-width font and preserves whitespace and line breaks.

**Syntax:**

```html
<pre>
    Preformatted text goes here
</pre>
```

**Example:**

```html
<!DOCTYPE html>
<html>
<head>
    <title>Preformatted Text Example</title>
</head>
<body>
    <h1>Preformatted Text Example</h1>
    <pre>
        This is preformatted text.
        It preserves spaces
        and line breaks.
        Indentation is also maintained.
    </pre>
</body>
</html>
```

### 9.2 Line Break (`<br>`)

The `<br>` tag inserts a line break within text. It is a self-closing tag.

**Syntax:**

```html
<p>First line<br>Second line</p>
```

**Example:**

```html
<!DOCTYPE html>
<html>
<head>
    <title>Line Break Example</title>
</head>
<body>
    <h1>Line Break Example</h1>
    <p>This is the first line. This is the second line. (No line break)</p>
    <p>
        This is the first line.<br>
        This is the second line.<br>
        This uses the line break tag.
    </p>
</body>
</html>
```

### 9.3 Horizontal Rule (`<hr>`)

The `<hr>` tag creates a horizontal line across the page. It is a self-closing tag.

**Syntax:**

```html
<hr>
```

**Example:**

```html
<!DOCTYPE html>
<html>
<head>
    <title>Horizontal Line Example</title>
</head>
<body>
    <h1>Horizontal Line Example</h1>
    <p>This is some text above the horizontal line.</p>
    <hr>
    <p>This is some text below the horizontal line.</p>
</body>
</html>
```

---

### Mini Project 3: Formatted Article Page

**Objective:** Create an article page using text formatting, line breaks, and horizontal rules.

**Step-by-Step Instructions:**

1. Create a new file named `project3.html`
2. Generate the basic HTML structure using `!` + `Tab`
3. Set the page title to `Science Article` inside the `<title>` tag
4. Inside the `<body>` tag, add the following in order:
   - Add the title `The Water Molecule` using `<h1>` tag
   - Add the author name in a paragraph, make it **italic** using `<i>` tag: `By: Dr. Science`
   - Add a `<hr>` tag to create a horizontal line
   - Add a paragraph with this content:
     - Write `Water` in **bold** using `<b>` tag
     - Write the chemical formula `H2O` using `<sub>` tag for the `2`
   - Add another paragraph about water properties
   - Add a `<hr>` tag
   - Add a section about Einstein's equation:
     - Use `<h2>` tag for heading `Famous Equation`
     - Write `E=mc2` where `2` is in **superscript** using `<sup>` tag
   - Add your name at the bottom in **bold** and **underlined** using `<b>` and `<u>` tags
   - Use `<br>` tag to add line breaks in contact information

**Solution:**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Science Article</title>
</head>
<body>
    <h1>The Water Molecule</h1>
    <p><i>By: Dr. Science</i></p>
    
    <hr>
    
    <p>
        <b>Water</b> is essential for all life on Earth. 
        The chemical formula for water is H<sub>2</sub>O, which means 
        each molecule contains two hydrogen atoms and one oxygen atom.
    </p>
    
    <p>
        Water exists in three states: solid (ice), liquid (water), 
        and gas (steam). It covers about 71% of the Earth's surface.
    </p>
    
    <hr>
    
    <h2>Famous Equation</h2>
    <p>
        Albert Einstein's famous equation is <b>E=mc<sup>2</sup></b>, 
        which shows the relationship between energy and mass.
    </p>
    
    <hr>
    
    <p>
        <b><u>Contact Author:</u></b><br>
        Email: dr.science@example.com<br>
        Phone: 9800000000<br>
        Location: Kathmandu, Nepal
    </p>
</body>
</html>
```

---

## 10. Images

The `<img>` tag embeds images in an HTML document. It is a self-closing tag.

**Required Attributes:**
- `src` - Path to the image file
- `alt` - Alternative text (for accessibility)

**Optional Attributes:**
- `width` - Width of the image
- `height` - Height of the image

**Syntax:**

```html
<img src="photo.jpg" alt="My Photo" width="300" height="400">
```

**Example:**

```html
<!DOCTYPE html>
<html>
<head>
    <title>Image Example</title>
</head>
<body>
    <h1>Image Example</h1>
    <img src="https://www.hetaudacitycollege.edu.np/_next/image?url=%2F_next%2Fstatic%2Fmedia%2Flogo.32bba284.jpg&w=96&q=85" alt="College Logo" width="200">
    <p>This is an example of an image in HTML.</p>
</body>
</html>
```

---

### Mini Project 4: Profile Card

**Objective:** Create a simple profile card with an image, formatted text, and sections.

**Step-by-Step Instructions:**

1. Create a new file named `project4.html`
2. Generate the basic HTML structure using `!` + `Tab`
3. Set the page title to `My Profile Card` inside the `<title>` tag
4. Inside the `<body>` tag, add the following in order:
   - Add a profile image using `<img>` tag:
     - Set `src` to any image URL (or use a placeholder)
     - Set `alt` to your name
     - Set `width` to `150`
   - Add your full name using `<h1>` tag
   - Add your role/title in **italic** using `<i>` tag inside a `<p>` tag (e.g., "Student | Web Developer")
   - Add a `<hr>` tag to separate sections
   - Create a `<div>` for "About" section:
     - Add `About` as heading using `<h2>` tag
     - Add a short description using `<p>` tag
   - Add a `<hr>` tag
   - Create a `<div>` for "Contact" section:
     - Add `Contact` as heading using `<h2>` tag
     - Add your email with the label in **bold** using `<b>` tag
     - Add your phone with the label in **bold** using `<b>` tag
     - Use `<br>` tags to separate contact lines

**Solution:**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Profile Card</title>
</head>
<body>
    <img src="https://www.hetaudacitycollege.edu.np/_next/image?url=%2F_next%2Fstatic%2Fmedia%2Flogo.32bba284.jpg&w=96&q=85" alt="Ram Sharma" width="150">
    <h1>Ram Sharma</h1>
    <p><i>Student | Web Developer | Tech Enthusiast</i></p>
    
    <hr>
    
    <div>
        <h2>About</h2>
        <p>
            I am a passionate computer science student who loves to build 
            websites and learn new technologies. Currently studying at 
            Hetauda City College.
        </p>
    </div>
    
    <hr>
    
    <div>
        <h2>Contact</h2>
        <p>
            <b>Email:</b> AntoneLee@example.com<br>
            <b>Phone:</b> 9841234567<br>
            <b>Location:</b> Hetauda, Nepal
        </p>
    </div>
</body>
</html>
```

---
