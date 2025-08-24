<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Enhanced HTML Form</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 2em;
      line-height: 1.6;
    }
    form {
      background: #f2f2f2;
      padding: 1em;
      border-radius: 5px;
      max-width: 500px;
    }
    label {
      display: block;
      margin-top: 1em;
    }
    input, select, textarea {
      width: 100%;
      padding: 0.5em;
      margin-top: 0.3em;
    }
    table {
      border-collapse: collapse;
      margin-top: 2em;
    }
    th, td {
      border: 1px solid #ccc;
      padding: 0.5em;
    }
    img {
      max-width: 100%;
      height: auto;
      margin-top: 1em;
    }
  </style>
</head>
<body>

  <header>
    <h1>User Registration</h1>
    <p>Please fill out the form below to register.</p>
  </header>

  <main>
    <form action="/submit" method="post" autocomplete="on">
      <label for="fullname">Full Name:</label>
      <input type="text" id="fullname" name="fullname" placeholder="John Doe" required autocomplete="name">

      <label for="email">Email:</label>
      <input type="email" id="email" name="email" placeholder="example@mail.com" required autocomplete="email">

      <label for="password">Password:</label>
      <input type="password" id="password" name="password" required minlength="6" placeholder="Enter a strong password">

      <label for="dob">Date of Birth:</label>
      <input type="date" id="dob" name="dob" required>

      <label for="country">Country:</label>
      <select id="country" name="country" required>
        <option value="">Select your country</option>
        <option value="usa">USA</option>
        <option value="uk">UK</option>
        <option value="canada">Canada</option>
      </select>

      <label for="bio">Short Bio:</label>
      <textarea id="bio" name="bio" placeholder="Tell us a bit about yourself..." rows="4"></textarea>

      <label for="readonly-field">Referral Code (readonly):</label>
      <input type="text" id="readonly-field" value="REF12345" readonly>

      <label>
        <input type="checkbox" name="terms" required> I agree to the terms and conditions
      </label>

      <button type="submit">Register</button>
    </form>

    <section>
      <h2>What You'll Get:</h2>
      <ul>
        <li>Access to premium content</li>
        <li>Monthly newsletter</li>
        <li>Exclusive discounts</li>
      </ul>
    </section>

    <section>
      <h2>Sample Data Table</h2>
      <table>
        <thead>
          <tr>
            <th>Plan</th>
            <th>Price</th>
            <th>Features</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Basic</td>
            <td>$10</td>
            <td>Email Support</td>
          </tr>
          <tr>
            <td>Pro</td>
            <td>$25</td>
            <td>Priority Support, Analytics</td>
          </tr>
        </tbody>
      </table>
    </section>

    <section>
      <h2>Welcome Video</h2>
      <video controls width="400">
        <source src="welcome.mp4" type="video/mp4">
        Your browser does not support the video tag.
      </video>
    </section>

    <section>
      <h2>Sample Image</h2>
      <img src="https://via.placeholder.com/400x200" alt="Sample placeholder image">
    </section>
  </main>

  <footer>
    <p>&copy; 2025 Your Company</p>
  </footer>

</body>
</html>
