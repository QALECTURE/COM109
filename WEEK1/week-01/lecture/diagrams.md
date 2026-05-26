# Week 1 Diagrams

These diagrams are designed for slides, handouts or quick whiteboard sketches.

## 1. Internet vs Web

```text
                 THE INTERNET
       Global network of connected devices

  +----------+      +----------+      +----------+
  | Laptop   |------| Router   |------| Server   |
  +----------+      +----------+      +----------+
       |                                  |
       |                                  |
  +----------+                      +----------+
  | Phone    |                      | Data     |
  |          |                      | Centre   |
  +----------+                      +----------+

 Services that use the Internet:

 +-------------+  +----------+  +----------+  +------+
 | World Wide  |  | Email    |  | SSH      |  | FTP  |
 | Web         |  |          |  |          |  |      |
 +-------------+  +----------+  +----------+  +------+
```

## 2. Browser-Server Request/Response Flow

```text
 Student enters URL:
 https://example.com

 +-----------+       HTTP/HTTPS Request       +-------------+
 | Browser   | -----------------------------> | Web Server  |
 | Chrome    |                                |             |
 +-----------+                                +-------------+
       ^                                             |
       |                                             |
       |        HTTP/HTTPS Response                  |
       |        HTML, CSS, JS, images                |
       +---------------------------------------------+

 Browser then renders the page for the user.
```

## 3. HTML + CSS + JavaScript Relationship

```text
 +------------------+
 | HTML             |
 | Structure        |
 | Headings, text,  |
 | images, forms    |
 +------------------+
          |
          v
 +------------------+
 | CSS              |
 | Presentation     |
 | Colours, layout, |
 | fonts, spacing   |
 +------------------+
          |
          v
 +------------------+
 | JavaScript       |
 | Behaviour        |
 | Clicks, updates, |
 | data, events     |
 +------------------+

 Together they create the user experience.
```

## 4. DOM Tree

```text
 document
    |
    +-- html
        |
        +-- head
        |   |
        |   +-- title
        |
        +-- body
            |
            +-- header
            |   |
            |   +-- h1
            |
            +-- main
            |   |
            |   +-- section
            |   |   |
            |   |   +-- h2
            |   |   +-- p
            |   |
            |   +-- section
            |       |
            |       +-- ul
            |           |
            |           +-- li
            |
            +-- footer
```

## 5. Static vs Dynamic Web Experience

```text
 STATIC PAGE

 +----------+       Request        +-------------+
 | Browser  | -------------------> | Server      |
 +----------+                      | index.html  |
      ^                            +-------------+
      |                                  |
      +---------- Same file each time ---+


 DYNAMIC PAGE

 +----------+       Request        +-------------+
 | Browser  | -------------------> | Server/App  |
 +----------+                      +-------------+
      ^                                  |
      |                                  v
      |                            +-------------+
      |                            | Database or |
      |                            | API data    |
      |                            +-------------+
      |                                  |
      +------ Page changes by user/data -+
```

## 6. GitHub Workflow

```text
 1. Edit file locally

 +----------------+
 | index.html     |
 | changed        |
 +----------------+
          |
          v
 2. Stage changes

 git add .
          |
          v
 3. Commit snapshot

 git commit -m "Add portfolio homepage"
          |
          v
 4. Push to GitHub

 git push
          |
          v
 +----------------+
 | GitHub Repo    |
 | Remote copy    |
 +----------------+
```

