Absolutely bro. **Restaurant website is much better for WT Lab** — it gives you more scope for cards, menu, buttons, responsive design, images, JS, and the 404 page, while still being easy enough to explain in viva.

 Let's make it:

 # 🍽️ Project: **The Rustic Plate**

 ### _Modern Restaurant & Café Website_

 The site will have:

 - Attractive full-screen food background
- Restaurant logo/name
- Navigation bar
- Hero section
- “View Menu” button
- Popular dishes
- About section
- Restaurant statistics
- Reservation/contact section
- JavaScript interaction
- Responsive mobile layout
- Custom 404 page
- GitHub Pages deployment

 For images, **Unsplash has dedicated restaurant, food, and restaurant-interior collections**, so you can quickly find suitable images there.  Unsplash+2

---

 # 1\. First create this folder

```
The-Rustic-Plate/
│
├── index.html
├── style.css
├── script.js
├── 404.html
│
└── images/
    ├── hero.jpg
    ├── pizza.jpg
    ├── pasta.jpg
    ├── burger.jpg
    ├── restaurant.jpg
    └── logo.png
```

 **Do this first.**

---

 # 2\. Images — what exactly to search

 Go to  Unsplash restaurant images  or  Pexels restaurant backgrounds .

 Search:

 ### `hero.jpg`

 Search:

```
dark restaurant food table aesthetic
```

 Pick a **wide landscape image** with some dark/empty space where white text can sit.

 ### `pizza.jpg`

 Search:

```
pizza restaurant food
```

 ### `pasta.jpg`

 Search:

```
pasta restaurant food
```

 ### `burger.jpg`

 Search:

```
gourmet burger restaurant
```

 ### `restaurant.jpg`

 Search:

```
modern restaurant interior warm lights
```

 ### `logo.png`

 Honestly, **don't waste time searching for a logo**.

 Make a very simple logo yourself using text:

```
RP
```

 or search:

```
restaurant logo png transparent
```

 If you find one, download it and rename it `logo.png`.

 For a student project, even a simple circular `RP` logo is completely fine.

---

 # 3\. `index.html`

 Create `index.html` and paste **this entire code**:

```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">

    <meta name="viewport"
          content="width=device-width, initial-scale=1.0">

    <title>The Rustic Plate</title>

    <link rel="stylesheet" href="style.css">
</head>

<body>

    <!-- Navigation -->

    <header>

        <nav class="navbar">

            <div class="logo">
                <img src="images/logo.png" alt="Restaurant Logo">
                <span>The Rustic Plate</span>
            </div>

            <div class="nav-links">

                <a href="#home">Home</a>
                <a href="#menu">Menu</a>
                <a href="#about">About</a>
                <a href="#contact">Contact</a>

            </div>

        </nav>

    </header>

    <!-- Hero Section -->

    <section class="hero" id="home">

        <div class="hero-content">

            <p class="tagline">
                FRESH • FLAVOUR • EXPERIENCE
            </p>

            <h1>
                Good Food.<br>
                <span>Good Mood.</span>
            </h1>

            <p>
                Welcome to The Rustic Plate — where fresh ingredients,
                delicious flavours and warm hospitality come together.
            </p>

            <a href="#menu" class="main-btn">
                Explore Our Menu
            </a>

        </div>

    </section>

    <!-- Menu Section -->

    <section class="menu" id="menu">

        <div class="section-heading">

            <p>OUR SPECIALITIES</p>

            <h2>Popular Dishes</h2>

            <span>
                Some of our favourite dishes prepared with love.
            </span>

        </div>

        <div class="food-cards">

            <!-- Pizza -->

            <div class="food-card">

                <img src="images/pizza.jpg"
                     alt="Italian Pizza">

                <div class="food-info">

                    <h3>Rustic Pizza</h3>

                    <p>
                        Fresh vegetables, mozzarella cheese
                        and our signature sauce.
                    </p>

                    <div class="food-bottom">

                        <strong>₹299</strong>

                        <button onclick="orderFood('Rustic Pizza')">
                            Order
                        </button>

                    </div>

                </div>

            </div>

            <!-- Pasta -->

            <div class="food-card">

                <img src="images/pasta.jpg"
                     alt="Creamy Pasta">

                <div class="food-info">

                    <h3>Creamy Pasta</h3>

                    <p>
                        Creamy homemade pasta with herbs
                        and parmesan cheese.
                    </p>

                    <div class="food-bottom">

                        <strong>₹249</strong>

                        <button onclick="orderFood('Creamy Pasta')">
                            Order
                        </button>

                    </div>

                </div>

            </div>

            <!-- Burger -->

            <div class="food-card">

                <img src="images/burger.jpg"
                     alt="Gourmet Burger">

                <div class="food-info">

                    <h3>Classic Burger</h3>

                    <p>
                        Juicy grilled patty with fresh vegetables
                        and special sauce.
                    </p>

                    <div class="food-bottom">

                        <strong>₹199</strong>

                        <button onclick="orderFood('Classic Burger')">
                            Order
                        </button>

                    </div>

                </div>

            </div>

        </div>

    </section>

    <!-- About Section -->

    <section class="about" id="about">

        <div class="about-content">

            <p class="tagline">OUR STORY</p>

            <h2>
                Made With Passion,<br>
                Served With Love.
            </h2>

            <p>
                The Rustic Plate is a modern restaurant focused on
                serving delicious food using fresh ingredients.
                Our goal is to create a comfortable place where
                friends and families can enjoy great food together.
            </p>

            <div class="stats">

                <div>
                    <strong>10+</strong>
                    <span>Years Experience</span>
                </div>

                <div>
                    <strong>50+</strong>
                    <span>Menu Items</span>
                </div>

                <div>
                    <strong>4.8</strong>
                    <span>Customer Rating</span>
                </div>

            </div>

        </div>

        <div class="about-image">

            <img src="images/restaurant.jpg"
                 alt="Restaurant Interior">

        </div>

    </section>

    <!-- Contact Section -->

    <section class="contact" id="contact">

        <p class="tagline">RESERVATIONS</p>

        <h2>Ready for a Great Meal?</h2>

        <p>
            Visit us and enjoy delicious food in a warm
            and comfortable atmosphere.
        </p>

        <button onclick="reserveTable()">
            Reserve a Table
        </button>

    </section>

    <!-- Footer -->

    <footer>

        <h3>The Rustic Plate</h3>

        <p>
            Good Food • Good Mood
        </p>

        <p>
            © 2026 The Rustic Plate | Web Technologies Lab
        </p>

    </footer>

    <script src="script.js"></script>

</body>

</html>
```

---

 # 4\. `style.css`

 Now create `style.css`:

```
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    scroll-behavior: smooth;
}

body {
    font-family: Arial, sans-serif;
    color: #222;
    background: #faf7f2;
}

/* ================= NAVBAR ================= */

header {
    position: absolute;
    width: 100%;
    z-index: 10;
}

.navbar {
    width: 90%;
    margin: auto;
    padding: 20px 0;

    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    display: flex;
    align-items: center;
    gap: 10px;

    color: white;
    font-size: 20px;
    font-weight: bold;
}

.logo img {
    width: 42px;
    height: 42px;
    object-fit: contain;
}

.nav-links {
    display: flex;
    gap: 30px;
}

.nav-links a {
    color: white;
    text-decoration: none;
    font-size: 15px;
}

.nav-links a:hover {
    color: #e9a23b;
}

/* ================= HERO ================= */

.hero {

    min-height: 100vh;

    background:
        linear-gradient(
            rgba(0,0,0,0.60),
            rgba(0,0,0,0.55)
        ),
        url("images/hero.jpg");

    background-size: cover;
    background-position: center;

    display: flex;
    align-items: center;

    padding: 100px 10%;

    color: white;
}

.hero-content {
    max-width: 650px;
}

.tagline {
    color: #e9a23b;

    font-size: 13px;

    letter-spacing: 3px;

    font-weight: bold;

    margin-bottom: 15px;
}

.hero h1 {
    font-size: 70px;

    line-height: 1.05;

    margin-bottom: 25px;
}

.hero h1 span {
    color: #e9a23b;
}

.hero-content > p:not(.tagline) {
    font-size: 18px;

    line-height: 1.7;

    margin-bottom: 30px;
}

.main-btn,
.contact button {

    display: inline-block;

    background: #e9a23b;

    color: #222;

    padding: 14px 25px;

    border-radius: 30px;

    border: none;

    text-decoration: none;

    font-weight: bold;

    cursor: pointer;
}

.main-btn:hover,
.contact button:hover {
    background: #f5bd64;
}

/* ================= MENU ================= */

.menu {
    padding: 90px 8%;
}

.section-heading {
    text-align: center;

    margin-bottom: 45px;
}

.section-heading > p {
    color: #c47d18;

    letter-spacing: 2px;

    font-size: 13px;

    font-weight: bold;
}

.section-heading h2 {
    font-size: 40px;

    margin: 10px 0;
}

.section-heading span {
    color: #777;
}

.food-cards {

    display: grid;

    grid-template-columns:
        repeat(3, 1fr);

    gap: 25px;
}

.food-card {

    background: white;

    border-radius: 15px;

    overflow: hidden;

    box-shadow:
        0 8px 25px
        rgba(0,0,0,0.08);

    transition: 0.3s;
}

.food-card:hover {
    transform: translateY(-8px);
}

.food-card img {

    width: 100%;

    height: 230px;

    object-fit: cover;
}

.food-info {
    padding: 22px;
}

.food-info h3 {

    font-size: 24px;

    margin-bottom: 10px;
}

.food-info p {

    color: #666;

    line-height: 1.5;

    margin-bottom: 20px;
}

.food-bottom {

    display: flex;

    justify-content: space-between;

    align-items: center;
}

.food-bottom strong {

    color: #c47d18;

    font-size: 22px;
}

.food-bottom button {

    background: #222;

    color: white;

    border: none;

    padding: 9px 18px;

    border-radius: 20px;

    cursor: pointer;
}

.food-bottom button:hover {
    background: #c47d18;
}

/* ================= ABOUT ================= */

.about {

    background: #241b16;

    color: white;

    padding: 90px 10%;

    display: grid;

    grid-template-columns:
        1fr 1fr;

    gap: 60px;

    align-items: center;
}

.about-content {
    max-width: 650px;
}

.about h2 {

    font-size: 43px;

    line-height: 1.2;

    margin-bottom: 25px;
}

.about-content > p:not(.tagline) {

    color: #d8cec7;

    line-height: 1.7;
}

.stats {

    display: flex;

    gap: 50px;

    margin-top: 40px;

    flex-wrap: wrap;
}

.stats div {

    display: flex;

    flex-direction: column;
}

.stats strong {

    color: #e9a23b;

    font-size: 30px;

    margin-bottom: 5px;
}

.stats span {
    color: #c8bdb5;
}

.about-image img {

    width: 100%;

    height: 400px;

    object-fit: cover;

    border-radius: 15px;
}

/* ================= CONTACT ================= */

.contact {

    text-align: center;

    padding: 85px 20px;
}

.contact h2 {

    font-size: 40px;

    margin-bottom: 15px;
}

.contact > p:not(.tagline) {

    color: #666;

    margin-bottom: 25px;
}

/* ================= FOOTER ================= */

footer {

    background: #15100d;

    color: white;

    text-align: center;

    padding: 30px;
}

footer h3 {
    color: #e9a23b;

    margin-bottom: 8px;
}

footer p {
    margin-top: 8px;

    color: #aaa;
}

/* ================= RESPONSIVE ================= */

@media (max-width: 768px) {

    .navbar {

        flex-direction: column;

        gap: 15px;
    }

    .nav-links {

        gap: 15px;

        flex-wrap: wrap;

        justify-content: center;
    }

    .hero {

        text-align: center;

        justify-content: center;
    }

    .hero h1 {

        font-size: 45px;
    }

    .food-cards {

        grid-template-columns: 1fr;
    }

    .about {

        grid-template-columns: 1fr;

        text-align: center;
    }

    .about-image {

        order: -1;
    }

    .stats {

        justify-content: center;
    }
}
```

---

 # 5\. `script.js`

 Very simple:

```
function orderFood(food) {

    alert(
        "Great choice! " +
        food +
        " has been added to your order."
    );

}

function reserveTable() {

    alert(
        "Thank you! Your table reservation request has been received."
    );

}
```

 That's enough.

 Don't make the JavaScript unnecessarily complicated. If madam asks what JS is doing, you can literally explain these two functions.

---

 # 6\. `404.html`

 This is specifically useful for **Experiment 6**.

```
<!DOCTYPE html>
<html lang="en">

<head>

    <meta charset="UTF-8">

    <meta name="viewport"
          content="width=device-width, initial-scale=1.0">

    <title>404 - Page Not Found</title>

    <link rel="stylesheet" href="style.css">

</head>

<body>

    <section class="hero">

        <div class="hero-content">

            <p class="tagline">
                ERROR 404
            </p>

            <h1>
                Oops!<br>
                <span>Page Not Found</span>
            </h1>

            <p>
                Sorry, the page you are looking for
                does not exist or may have been moved.
            </p>

            <a href="index.html" class="main-btn">
                Return Home
            </a>

        </div>

    </section>

</body>

</html>
```

---

 # 7\. What the final website looks like

 Your website flow is:

```
┌─────────────────────────────────────────────┐
│ RP  THE RUSTIC PLATE     Home Menu About   │
│                                             │
│                                             │
│       FRESH • FLAVOUR • EXPERIENCE          │
│                                             │
│       GOOD FOOD.                            │
│       GOOD MOOD.                            │
│                                             │
│       [ Explore Our Menu ]                  │
│                                             │
└─────────────────────────────────────────────┘

              POPULAR DISHES

      ┌────────┐  ┌────────┐  ┌────────┐
      │ PIZZA  │  │ PASTA  │  │ BURGER │
      │        │  │        │  │        │
      │ ₹299   │  │ ₹249   │  │ ₹199   │
      │ [Order]│  │ [Order]│  │ [Order]│
      └────────┘  └────────┘  └────────┘

       MADE WITH PASSION, SERVED WITH LOVE

       10+        50+        4.8
       Years      Items      Rating

              [Restaurant image]

              READY FOR A GREAT MEAL?

                 [Reserve]
```

 It will look like a **proper restaurant landing page**, not like a random beginner HTML exercise.

---

 # 8\. Run it locally

 In VS Code:

 1. Open the `The-Rustic-Plate` folder.
2. Make sure all 5 images are inside `images`.
3. Open `index.html`.
4. Use **Live Server** if you have it.
5. Open the site in Chrome.

 Check:

 - Home button
- Menu button
- About button
- Contact button
- Order buttons
- Reserve button
- Mobile responsiveness

---

 # 9\. VERY IMPORTANT — test the images

 Your filenames need to match **exactly**:

```
images/hero.jpg
images/pizza.jpg
images/pasta.jpg
images/burger.jpg
images/restaurant.jpg
images/logo.png
```

 If you download:

```
pizza-food.jpeg
```

 rename it:

```
pizza.jpg
```

 **only if you're actually converting/saving it as JPEG**. Don't merely change `.webp` to `.jpg` — browsers can sometimes handle the original format, but the extension should match the actual file.

---

 # 10\. Now Experiment 6

 Your experiment becomes much more natural with this project.

 ## Experiment No. 6

 ### Aim

 > To deploy a responsive web application on a cloud hosting platform, configure public access, implement basic error handling, and verify its functionality in a live environment.

 ### Project Name

 > **The Rustic Plate – Restaurant Website**

 ### Problem Statement

 > Develop and deploy a responsive restaurant web application using HTML, CSS and JavaScript. Configure public access using a cloud hosting platform, implement basic error handling and verify the application in a live environment.

---

 # 11\. Software Requirements

 | Requirement | Description |
| --- | --- |
| Code Editor | Visual Studio Code |
| Browser | Google Chrome |
| Programming | HTML, CSS, JavaScript |
| Version Control | Git and GitHub |
| Hosting | GitHub Pages |
| Internet | Required |
| OS | Windows/Linux/macOS |

---

 # 12\. Project structure

 Put this in your practical:

```
The-Rustic-Plate/
│
├── index.html
├── style.css
├── script.js
├── 404.html
│
└── images/
    ├── hero.jpg
    ├── pizza.jpg
    ├── pasta.jpg
    ├── burger.jpg
    ├── restaurant.jpg
    └── logo.png
```

---

 # 13\. Step 1 — Develop responsive web application

 Write:

 > A responsive restaurant website named **The Rustic Plate** was developed using HTML, CSS and JavaScript. The website contains a navigation bar, hero section, food menu, restaurant information, contact section and footer. CSS media queries were used to make the website responsive on mobile devices.

 Your CSS has:

```
@media (max-width: 768px)
```

 That is your **responsive design implementation**.

---

 # 14\. Step 2 — Create GitHub repository

 Go to  GitHub .

 Create:

```
The-Rustic-Plate
```

 Make it **Public**.

 Upload:

```
index.html
style.css
script.js
404.html
images/
```

 Commit the files.

---

 # 15\. Or use Git commands

 If madam expects commands, use:

```
git init
```

 Then:

```
git add .
```

 Then:

```
git commit -m "Initial restaurant website"
```

 Then:

```
git branch -M main
```

 Then connect your GitHub repository:

```
git remote add origin YOUR_GITHUB_REPOSITORY_URL
```

 Then:

```
git push -u origin main
```

---

 # 16\. Step 3 — Deploy using GitHub Pages

 Inside your GitHub repository:

 **Settings**

 → **Pages**

 Under:

 ### Build and deployment

 Select:

```
Source: Deploy from a branch
Branch: main
Folder: / (root)
```

 Then:

 **Save**

 Wait for deployment.

 GitHub will give you something like:

```
https://yourusername.github.io/The-Rustic-Plate/
```

 That's your **public URL**.

---

 # 17\. Step 4 — Hosting configuration

 Write:

 > GitHub Pages was configured as the hosting platform. The `main` branch was selected as the deployment branch and the root folder was selected as the publishing directory. After successful deployment, GitHub generated a public HTTPS URL through which the restaurant website could be accessed.

---

 # 18\. Step 5 — Error handling

 Your project has a proper:

```
404.html
```

 So test it.

 Suppose your real URL is:

```
https://abc.github.io/The-Rustic-Plate/
```

 Now deliberately open:

```
https://abc.github.io/The-Rustic-Plate/random
```

 You should see:

```
ERROR 404

Oops!
Page Not Found

Sorry, the page you are looking for
does not exist or may have been moved.

[ Return Home ]
```

 **Take a screenshot.**

 That's one of your best screenshots for Experiment 6.

---

 # 19\. What to say about 500 error

 Don't claim that your HTML website has implemented a real server-side 500 handler.

 If madam asks:

 > “Where is your 500 error handling?”

 Say:

 > **“This is a static web application hosted on GitHub Pages, so server-side 500 errors are handled by the hosting infrastructure. I implemented a custom 404 page for invalid URLs and application-level feedback using JavaScript.”**

 That's a much better answer than pretending your `alert()` is a server error.

---

 # 20\. Step 6 — Testing

 Put this table directly in your practical:

 | Test Case | Expected Output | Result |
| --- | --- | --- |
| Open public URL | Restaurant website loads | Pass |
| Open website on mobile | Responsive layout displayed | Pass |
| Click Home | Home section displayed | Pass |
| Click Menu | Menu section displayed | Pass |
| Click Order | Order message displayed | Pass |
| Click Reserve | Reservation message displayed | Pass |
| Enter invalid URL | Custom 404 page displayed | Pass |
| Check images | Food and restaurant images load | Pass |
| Test navigation | Navigation works correctly | Pass |

---

 # 21\. Screenshots — don't waste time

 Take **exactly these**:

 ### Screenshot 1

 VS Code:

```
The-Rustic-Plate
├── index.html
├── style.css
├── script.js
├── 404.html
└── images
```

 ### Screenshot 2

 Your beautiful homepage.

 ### Screenshot 3

 Menu section showing:

```
Pizza | Pasta | Burger
```

 ### Screenshot 4

 GitHub repository with files.

 ### Screenshot 5

 GitHub Pages deployment/settings.

 ### Screenshot 6

 Live website URL.

 ### Screenshot 7

 404 page after entering a fake URL.

 That's plenty.

---

 # 22\. Final conclusion for Experiment 6

 Put:

 > **Conclusion:**\
>  The responsive restaurant web application **The Rustic Plate** was successfully developed using HTML, CSS and JavaScript. The application was uploaded to GitHub and deployed using GitHub Pages. A public HTTPS URL was generated successfully. Responsive design was tested on different screen sizes and a custom 404 error page was implemented for invalid URLs. The major website functions and navigation were tested successfully in the live environment. Hence, the objectives of Experiment 6 were successfully achieved.

---

 # 23\. Your viva — memorize these 7 answers

 If madam suddenly asks you questions, you're covered:

 **Q: Which technologies did you use?**

 > HTML, CSS and JavaScript.

 **Q: Why did you use CSS media queries?**

 > To make the website responsive on different screen sizes such as desktop, tablet and mobile.

 **Q: What is GitHub Pages?**

 > It is a static web hosting service that can host websites directly from a GitHub repository.

 **Q: What is your 404 page?**

 > `404.html`. It displays a custom page when a requested URL does not exist.

 **Q: What does JavaScript do in your project?**

 > It handles user interactions such as the Order and Reserve Table buttons.

 **Q: Is your website static or dynamic?**

 > It is a static web application because the content is stored in HTML, CSS and JavaScript files and there is no server-side database.

 **Q: How did you make it responsive?**

 > I used CSS media queries with a breakpoint at 768 pixels and changed the navigation, cards and sections for smaller screens.

---

 ## 🔥 The fastest route right now

 Don't overthink it.

 **Do this in order:**

 1. Create `The-Rustic-Plate` folder.
2. Create the 4 code files above.
3. Create `images` folder.
4. Download **5 images**.
5. Rename them exactly.
6. Paste the code.
7. Open in Chrome.
8. Fix any image filename issue.
9. Create GitHub repo.
10. Upload folder.
11. Enable GitHub Pages.
12. Test live URL.
13. Test `/random` for 404.
14. Take the 7 screenshots.
15. Put the Experiment 6 write-up above in your journal.

 For the images, **don't spend 30 minutes searching Google**. Unsplash's restaurant/food collections already have thousands of suitable photos, and Pexels also has a large restaurant-background collection.  Unsplash+2

 And bro, **this version is better for your lab**: it looks like a proper mini-project, but if your mam asks you to explain any part, every piece is simple enough to explain yourself.