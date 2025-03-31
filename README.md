# CSS Layouts and Responsive Design

## Objectives

Implement Flexbox and Grid for layout design.
Make the webpage responsive using media queries.
Ensure proper alignment and spacing.

## Instructions

- use Flexbox or CSS Grid.
- Add a navigation bar and structure the content.
- Use media queries to adjust layout for mobile, tablet, and desktop.

>[!NOTE]
>  - Include at least:
>  - navigation bar
>  - media queries

# Tasks

- Apply Flexbox or Grid for layout.
- Make the page responsive.
- Test across different screen sizes.

Happy Coding! 💻✨
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Layout</title>
    <style>
        body {
            font-family: sans-serif;
            margin: 0;
            padding: 0;
        }

        nav {
            background-color: #333;
            color: white;
            padding: 10px 20px;
        }

        nav ul {
            list-style: none;
            padding: 0;
            margin: 0;
            display: flex;
        }

        nav li {
            margin-right: 20px;
        }

        nav a {
            color: white;
            text-decoration: none;
        }

        .container {
            display: flex;
            flex-wrap: wrap;
            padding: 20px;
        }

        .sidebar {
            background-color: #f0f0f0;
            padding: 20px;
            flex: 1;
            min-width: 200px;
        }

        .content {
            background-color: #e0e0e0;
            padding: 20px;
            flex: 3;
            min-width: 300px;
        }

        /* Media Queries */

        @media (max-width: 768px) { /* Tablet and smaller */
            .container {
                flex-direction: column;
            }

            .sidebar, .content {
                width: 100%;
            }
        }

        @media (max-width: 480px) { /* Mobile */
            nav ul {
                flex-direction: column;
            }

            nav li {
                margin-right: 0;
                margin-bottom: 10px;
            }
        }
    </style>
</head>
<body>

    <nav>
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">About</a></li>
            <li><a href="#">Services</a></li>
            <li><a href="#">Contact</a></li>
        </ul>
    </nav>

    <div class="container">
        <div class="sidebar">
            <h2>Sidebar</h2>
            <p>This is the sidebar content. It can contain navigation links, advertisements, or other relevant information.</p>
        </div>
        <div class="content">
            <h2>Main Content</h2>
           <p>Kenya is a country in East Africa with coastline on the Indian Ocean. It encompasses savannah, lakelands, the dramatic Great Rift Valley and mountain highlands. It's also home to wildlife like lions, elephants and rhinos.</p>
            <p>More content goes here...</p>
        </div>
    </div>

</body>
</html>
