<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bookstore</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #333;
            color: white;
            padding: 10px;
            text-align: center;
        }
        header a {
            color: white;
            text-decoration: none;
            margin: 0 15px;
        }
        .book-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-around;
            padding: 20px;
        }
        .book {
            background-color: white;
            border: 1px solid #ddd;
            border-radius: 5px;
            margin: 10px;
            padding: 10px;
            width: 200px;
        }
        .book img {
            width: 100%;
            height: auto;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
        form {
            margin: 20px;
        }
        form input, form select, form textarea {
            display: block;
            margin-bottom: 10px;
        }
        form button {
            background-color: #333;
            color: white;
            border: none;
            padding: 10px 20px;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <header>
        <a href="#new-arrivals">New Arrivals</a>
        <a href="#categories">Categories</a>
        <a href="#contact">Contact</a>
    </header>

    <div class="book-container">
        <!-- Example book -->
        <div class="book">
            <img src="book-image.jpg" alt="Book Image">
            <h3>Book Title</h3>
            <p>Author: John Doe</p>
            <p>Genre: Fiction</p>
            <p>Summary: A thrilling adventure...</p>
        </div>
        <!-- Add more books as needed -->
    </div>

    <footer>
        &copy; 2023 Bookstore. All rights reserved.
    </footer>

    <form id="bookstoreForm">
        <label for="name">Name:</label>
        <input type="text" id="name" name="name">

        <label for="email">Email:</label>
        <input type="email" id="email" name="email">

        <label for="message">Message:</label>
        <textarea id="message" name="message"></textarea>

        <label for="category">Category:</label>
        <select id="category" name="category">
            <option value="fiction">Fiction</option>
            <option value="non-fiction">Non-Fiction</option>
            <option value="science">Science</option>
        </select>

        <label for="file">Upload File:</label>
        <input type="file" id="file" name="file">

        <button type="submit">Submit</button>
    </form>

    <script>
        document.getElementById('bookstoreForm').addEventListener('submit', function(event) {
            event.preventDefault();
            // Handle form submission here
            alert('Form submitted!');
        });
    </script>
</body>
</html>
