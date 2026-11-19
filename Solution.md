1. HTML Code

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Magazine Layout</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <div class="container">

        <header>
            <h1>THE DAILY NEWS</h1>
            <p>Your Daily Dose of Information</p>
        </header>

        <nav>
            <a href="#">Home</a>
            <a href="#">World</a>
            <a href="#">Technology</a>
            <a href="#">Sports</a>
            <a href="#">Entertainment</a>
        </nav>

        <main>
            <article>
                <h2>Technology is Changing the World</h2>
                <img src="https://images.unsplash.com/photo-1519389950473-47ba0277781c?w=900"
                     alt="People working with technology">

                <p>
                    Technology has become an important part of our daily lives.
                    From smartphones to artificial intelligence, new innovations
                    are changing how people communicate, work and learn.
                </p>

                <p>
                    Modern technology makes information more accessible and
                    helps businesses grow. The future will bring even more
                    exciting developments in science and technology.
                </p>

                <a href="#">Read More →</a>
            </article>
        </main>

        <aside>
            <h2>Latest News</h2>
            <ul>
                <li>New AI Technologies Released</li>
                <li>Global Education Updates</li>
                <li>Latest Sports Headlines</li>
                <li>Science and Innovation News</li>
            </ul>

            <h2>Popular Posts</h2>
            <p>Top Technology Trends of 2026</p>
            <p>Future of Digital Education</p>
        </aside>

        <footer>
            <p>© 2026 The Daily News | All Rights Reserved</p>
        </footer>

    </div>

</body>
</html>
2. CSS Code (style.css)

css

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background-color: #f2f2f2;
    color: #333;
    line-height: 1.6;
}

.container {
    width: 90%;
    margin: 20px auto;

    display: grid;

    grid-template-columns: 3fr 1fr;

    grid-template-rows: auto auto 1fr auto;

    grid-template-areas:
        "header header"
        "nav nav"
        "main sidebar"
        "footer footer";

    gap: 15px;
}

/* Header */
header {
    grid-area: header;
    background-color: #172554;
    color: white;
    text-align: center;
    padding: 30px;
}

/* Navigation */
nav {
    grid-area: nav;
    background-color: #2563eb;
    padding: 15px;
    text-align: center;
}

nav a {
    color: white;
    text-decoration: none;
    margin: 0 15px;
    font-weight: bold;
}

/* Main Article */
main {
    grid-area: main;
    background-color: white;
    padding: 25px;
}

article h2 {
    color: #172554;
    margin-bottom: 15px;
}

article img {
    width: 100%;
    height: 300px;
    object-fit: cover;
    margin-bottom: 15px;
}

article p {
    margin-bottom: 15px;
}

article a {
    color: #2563eb;
    text-decoration: none;
    font-weight: bold;
}

/* Sidebar */
aside {
    grid-area: sidebar;
    background-color: #e2e8f0;
    padding: 20px;
}

aside h2 {
    margin-bottom: 10px;
    color: #172554;
}

aside ul {
    padding-left: 20px;
    margin-bottom: 20px;
}

aside li {
    margin-bottom: 10px;
}

/* Footer */
footer {
    grid-area: footer;
    background-color: #172554;
    color: white;
    text-align: center;
    padding: 20px;
}

/* Responsive Design */
@media (max-width: 768px) {
    .container {
        width: 95%;

        grid-template-columns: 1fr;

        grid-template-areas:
            "header"
            "nav"
            "main"
            "sidebar"
            "footer";
    }

    nav a {
        display: inline-block;
        margin: 5px;
    }
}
3. Expected Layout Design
THE DAILY NEWS
Your Daily Dose of Information

Home　 World　 Technology　 Sports

Main Article

2026 How to Pay for a Computer Science Master's Degree with Financial Aid | Research.com
 
Technology is Changing the World

Technology is transforming our daily lives...

Latest News

• AI Technologies

• Education Updates

• Sports News

Popular Posts

• Technology Trends

© 2026 The Daily News | All Rights Reserved

4. Explanation of CSS Grid Properties
Property

Purpose

display: grid

Creates a grid container.

grid-template-columns

Defines column sizes.

grid-template-rows

Defines row sizes.

grid-template-areas

Defines named layout areas.

grid-area

Assigns an element to a named area.

gap

Adds space between grid sections.

5. Assignment Requirements Completed

Created header section.

Created navigation section.

Created main article section.

Created sidebar section.

Created footer section.

Defined a CSS Grid container.

Used grid-template-areas.

Assigned named grid areas.

Gave the main article more space than the sidebar using 3fr 1fr.

Added responsive design for mobile screens.
6. Conclusion
In this assignment, I created a magazine-style webpage using CSS Grid Layout. I used grid-template-areas to organize the header, navigation, main article, sidebar, and footer. I also used different column sizes to give more space to the main article and added responsive design to make the webpage mobile-friendly.