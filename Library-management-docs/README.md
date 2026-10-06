<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Library Management System</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0; padding: 0;
      background: #f4f4f4;
    }
    header {
      background: #2c3e50;
      color: #fff;
      padding: 15px;
      text-align: center;
    }
    nav {
      background: #34495e;
      padding: 10px;
      text-align: center;
    }
    nav a {
      color: #fff;
      margin: 0 15px;
      text-decoration: none;
    }
    nav a:hover {
      text-decoration: underline;
    }
    section {
      padding: 20px;
    }
    table {
      width: 100%;
      border-collapse: collapse;
      margin-top: 15px;
    }
    table, th, td {
      border: 1px solid #ccc;
    }
    th, td {
      padding: 10px;
      text-align: center;
    }
    form {
      margin-top: 15px;
    }
    footer {
      background: #2c3e50;
      color: #fff;
      text-align: center;
      padding: 10px;
      position: fixed;
      bottom: 0; width: 100%;
    }
  </style>
</head>
<body>
  <header>
    <h1>Library Management System</h1>
  </header>

  <nav>
    <a href="#books">Books</a>
    <a href="#members">Members</a>
    <a href="#issue">Issue Book</a>
    <a href="#reports">Reports</a>
  </nav>

  <section id="books">
    <h2>Books</h2>
    <table>
      <tr>
        <th>ID</th>
        <th>Title</th>
        <th>Author</th>
        <th>Status</th>
      </tr>
      <tr>
        <td>B001</td>
        <td>The Great Gatsby</td>
        <td>F. Scott Fitzgerald</td>
        <td>Available</td>
      </tr>
      <tr>
        <td>B002</td>
        <td>1984</td>
        <td>George Orwell</td>
        <td>Issued</td>
      </tr>
    </table>
  </section>

  <section id="members">
    <h2>Members</h2>
    <table>
      <tr>
        <th>ID</th>
        <th>Name</th>
        <th>Membership</th>
        <th>Status</th>
      </tr>
      <tr>
        <td>M001</td>
        <td>Arun Kumar</td>
        <td>Student</td>
        <td>Active</td>
      </tr>
      <tr>
        <td>M002</td>
        <td>Priya Sharma</td>
        <td>Faculty</td>
        <td>Active</td>
      </tr>
    </table>
  </section>

  <section id="issue">
    <h2>Issue Book</h2>
    <form>
      <label for="member">Select Member:</label>
      <select id="member" name="member">
        <option>Arun Kumar - M001</option>
        <option>Priya Sharma - M002</option>
      </select><br><br>

      <label for="book">Select Book:</label>
      <select id="book" name="book">
        <option>The Great Gatsby - B001</option>
        <option>1984 - B002</option>
      </select><br><br>

      <label for="date">Issue Date:</label>
      <input type="date" id="date" name="date"><br><br>

      <button type="submit">Issue Book</button>
    </form>
  </section>

  <section id="reports">
    <h2>Reports</h2>
    <p>Generate book issue/return reports here.</p>
  </section>

  <footer>
    <p>&copy; 2026 Library Management System</p>
  </footer>

  <script>
    // Example JavaScript for form submission
    document.querySelector("form").addEventListener("submit", function(e) {
      e.preventDefault();
      alert("Book issued successfully!");
    });
  </script>
</body>
</html>
