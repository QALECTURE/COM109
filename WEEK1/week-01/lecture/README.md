# Week 1 Lecture Notes

# Introduction to the Web, HTML and GitHub

These notes are designed for beginner Bachelor’s students. Each topic includes a simple explanation, a technical explanation, an analogy, a short teaching prompt and a mini question.

## 1. What Is the Internet?

**Simple explanation:**  
The Internet is a huge global network of connected computers, phones, servers, cables, routers and data centres. It lets devices send information to each other.

**Technical explanation:**  
The Internet is a network of networks that uses agreed communication rules, especially TCP/IP, to move data between devices. It supports many services, including the Web, email, file transfer, messaging, gaming and video streaming.

**Real-world analogy:**  
Think of the Internet like the road system. Roads connect houses, shops, offices and cities. Different vehicles can use the roads for different purposes.

**What to say in class:**  
"The Internet is the infrastructure. It is the thing that connects devices together. The Web is only one service that runs on top of it."

**Mini question:**  
Can you name three things you use every day that need the Internet?

## 2. What Is the World Wide Web?

**Simple explanation:**  
The World Wide Web, usually called the Web, is a collection of websites and webpages that you access using a browser.

**Technical explanation:**  
The Web is an information system built on URLs, HTTP/HTTPS, HTML documents, browsers and web servers. Webpages can link to each other using hyperlinks.

**Real-world analogy:**  
If the Internet is the road system, the Web is one type of service using the roads, like delivery vans carrying webpages to your browser.

**What to say in class:**  
"When you open Chrome and visit the BBC, Amazon or GitHub, you are using the Web. When an app sends a notification or a game connects online, it may be using the Internet without using normal webpages."

**Mini question:**  
Is Google Search part of the Web? Why?

## 3. Difference Between Internet and Web

**Simple explanation:**  
The Internet is the connection system. The Web is a service that uses that connection system.

**Technical explanation:**  
The Internet provides the networking infrastructure. The Web uses protocols such as HTTP and HTTPS to request and receive resources such as HTML pages, images, CSS files and JavaScript files.

**Real-world analogy:**  
The Internet is like electricity in a building. The Web is like one appliance using that electricity.

**What to say in class:**  
"All Web activity uses the Internet, but not all Internet activity is the Web. Email, SSH, FTP and some messaging systems are Internet services too."

**Mini question:**  
Is WhatsApp the same as the Web? What does it use from the Internet?

## 4. What Is a Browser?

**Simple explanation:**  
A browser is an app that lets users visit websites and view webpages.

**Technical explanation:**  
A browser sends requests to web servers, receives resources such as HTML, CSS and JavaScript, parses them, builds the DOM, applies styles, runs scripts and displays the final page to the user.

**Real-world analogy:**  
The browser is like a translator and builder. It receives instructions and materials, then turns them into a page users can see and interact with.

**What to say in class:**  
"Chrome, Edge, Firefox and Safari are not the Web itself. They are tools we use to access the Web."

**Mini question:**  
Which browser do you use most, and why?

## 5. What Is a Web Server?

**Simple explanation:**  
A web server is a computer that stores website files and sends them to browsers when requested.

**Technical explanation:**  
A web server listens for HTTP or HTTPS requests and responds with resources such as HTML documents, images, CSS, JavaScript, JSON data or error messages.

**Real-world analogy:**  
A web server is like a restaurant kitchen. The browser places an order, and the server sends back what was requested.

**What to say in class:**  
"When you visit Netflix or GitHub, your browser is asking servers somewhere else for files and data."

**Mini question:**  
What might happen if a web server is offline?

## 6. What Is HTTP/HTTPS?

**Simple explanation:**  
HTTP is the language browsers and web servers use to talk to each other. HTTPS is the secure version.

**Technical explanation:**  
HTTP stands for Hypertext Transfer Protocol. It defines how clients request resources and how servers respond. HTTPS adds encryption using TLS, which helps protect data from being read or changed during transfer.

**Real-world analogy:**  
HTTP is like sending a postcard. HTTPS is like sending the message in a sealed envelope.

**What to say in class:**  
"When you log in to Monzo, Revolut, Amazon or your university account, HTTPS matters because your data must be protected."

**Mini question:**  
Why should login pages use HTTPS?

## 7. What Happens When a Student Types a URL in the Browser?

**Simple explanation:**  
The browser finds the correct server, asks for the webpage, receives files, and displays the page.

**Technical explanation:**  
The browser reads the URL, may use DNS to find the server IP address, opens a connection, sends an HTTP/HTTPS request, receives a response, downloads linked resources, builds the DOM and renders the page.

**Real-world analogy:**  
Typing a URL is like entering a delivery address. The system works out where to go, collects the package and brings it back.

**What to say in class:**  
"A webpage appearing in the browser feels instant, but many steps happen quickly in the background."

**Mini question:**  
What do you think DNS is responsible for?

## 8. What Is HTML?

**Simple explanation:**  
HTML is the language used to structure content on a webpage.

**Technical explanation:**  
HTML stands for HyperText Markup Language. It uses elements and tags to describe content such as headings, paragraphs, links, images, lists, forms and page sections.

**Real-world analogy:**  
HTML is like the skeleton of a webpage. It gives the page structure.

**What to say in class:**  
"HTML tells the browser what each piece of content means. This is a heading, this is a paragraph, this is a link, this is a form."

**Mini question:**  
What HTML tag would you use for the most important heading on a page?

## 9. What Is CSS?

**Simple explanation:**  
CSS controls how a webpage looks.

**Technical explanation:**  
CSS stands for Cascading Style Sheets. It defines visual presentation, including colours, fonts, spacing, layout, borders, responsiveness and animation.

**Real-world analogy:**  
CSS is like clothing and interior design. It changes appearance without changing the underlying structure.

**What to say in class:**  
"HTML gives the content meaning. CSS makes it visually clear, professional and usable."

**Mini question:**  
What visual features make a website feel easy to use?

## 10. What Is JavaScript?

**Simple explanation:**  
JavaScript adds behaviour and interactivity to webpages.

**Technical explanation:**  
JavaScript is a programming language that runs in the browser. It can respond to events, update the DOM, validate forms, fetch data and create interactive experiences.

**Real-world analogy:**  
JavaScript is like the control system in a car. It reacts when something happens, such as pressing a button.

**What to say in class:**  
"When TikTok loads more videos, Amazon updates a basket, or Deliveroo tracks an order on a map, JavaScript is likely involved."

**Mini question:**  
What interactive feature have you used on a website today?

## 11. How HTML, CSS and JavaScript Work Together

**Simple explanation:**  
HTML creates the content, CSS styles it, and JavaScript makes it interactive.

**Technical explanation:**  
The browser parses HTML into the DOM, applies CSS rules to determine presentation, and executes JavaScript to update content, respond to events or communicate with servers.

**Real-world analogy:**  
For a house: HTML is the structure, CSS is the decoration, and JavaScript is the electricity and smart controls.

**What to say in class:**  
"A strong frontend developer understands all three layers. In Week 1, we start with the structure."

**Mini question:**  
If a button looks nice but does nothing, which technology is probably missing?

## 12. Static Web Pages vs Dynamic Web Pages

**Simple explanation:**  
A static page shows the same content until someone edits the files. A dynamic page can change based on data, users or interaction.

**Technical explanation:**  
Static pages are often served as fixed HTML, CSS and JavaScript files. Dynamic pages may be generated by server-side code, updated by client-side JavaScript, or populated using API data.

**Real-world analogy:**  
A static page is like a printed poster. A dynamic page is like a live departure board at a train station.

**What to say in class:**  
"Your Week 1 portfolio is mostly static. Later, JavaScript can make pages respond and update."

**Mini question:**  
Is a Netflix recommendations page static or dynamic? Why?

## 13. Introduction to DOM

**Simple explanation:**  
The DOM is the browser's live version of the HTML page.

**Technical explanation:**  
DOM stands for Document Object Model. It represents the webpage as a tree of objects that JavaScript can read and change.

**Real-world analogy:**  
The DOM is like a family tree for the page. Elements have parents, children and siblings.

**What to say in class:**  
"When we inspect a page in DevTools, we are looking at the browser's structured version of the document."

**Mini question:**  
Why might JavaScript need to find an element in the DOM?

## 14. Why Frontend Development Matters in Industry

**Simple explanation:**  
Frontend development shapes what users see, understand and interact with.

**Technical explanation:**  
Frontend developers build user interfaces, connect to APIs, improve accessibility, optimise performance and create responsive layouts for different devices.

**Real-world analogy:**  
Frontend is the shop floor of a digital product. If users cannot find, understand or trust it, the product fails.

**What to say in class:**  
"A bank app, booking system or online shop might have powerful backend systems, but users judge the product through the interface."

**Mini question:**  
What makes you leave a website quickly?

## 15. London/UK Job Relevance of Frontend Skills

**Simple explanation:**  
Frontend skills are useful for many technology, design, business and media roles in the UK.

**Technical explanation:**  
Employers often expect junior developers, UX engineers, digital analysts, content designers and full-stack developers to understand HTML, CSS, JavaScript, Git and browser tools.

**Real-world analogy:**  
Knowing frontend basics is like being able to read and write the language of digital products.

**What to say in class:**  
"London and the wider UK tech market include fintech, retail, media, transport, health and public sector employers. Companies like Monzo, Revolut, BBC, Tesco, Just Eat, Deliveroo and many agencies rely on web skills."

**Mini question:**  
Which industry could you imagine using web development in?

## 16. How GitHub Is Used by Developers

**Simple explanation:**  
GitHub is a place where developers store, share and collaborate on code.

**Technical explanation:**  
GitHub hosts Git repositories. Developers use commits to save versions, branches to work safely, pull requests to review changes and issues to track tasks or bugs.

**Real-world analogy:**  
GitHub is like Google Drive for code, but with a detailed history of every meaningful change and tools for teamwork.

**What to say in class:**  
"GitHub is also part of your professional identity. A portfolio and GitHub profile can show employers what you can build."

**Mini question:**  
Why might a team want to review code before merging it?

