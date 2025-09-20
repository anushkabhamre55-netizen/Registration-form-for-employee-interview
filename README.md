<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Registration Page</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f0f0f0;
      text-align: center;
      padding: 20px;
    }

    .box {
      background: white;
      max-width: 350px;
      margin: auto;
      padding: 20px;
      border-radius: 8px;
      box-shadow: 0 0 8px rgba(0,0,0,0.2);
    }

    input[type="checkbox"] {
      display: none;
    }

    /* Front page by default */
    .welcome {
      display: block;
    }

    /* Hide welcome when checked */
    #show:checked ~ .box .welcome {
      display: none;
    }

    /* Show form when checked */
    #show:checked ~ .box .form {
      display: block;
    }

    .form {
      display: none;
      text-align: left;
    }

    input, button {
      width: 100%;
      padding: 10px;
      margin: 8px 0;
      border: 1px solid #ccc;
      border-radius: 4px;
    }

    button {
      background: #4CAF50;
      color: white;
      border: none;
      cursor: pointer;
    }

    button:hover {
      background: #45a049;
    }

    label.start {
      display: inline-block;
      padding: 10px 20px;
      background: #4CAF50;
      color: white;
      border-radius: 4px;
      cursor: pointer;
    }
  </style>
</head>
<body>

  <input type="checkbox" id="show">

  <div class="box">
    <!-- Front Page -->
    <div class="welcome">
      <h2>Welcome</h2>
      <p>Click below to start your registration.</p>
      <label for="show" class="start">Start Registration</label>
    </div>

    <!-- Registration Form -->
    <div class="form">
      <h2>Register</h2>
      <form>
        <input type="text" placeholder="Firstname" required>
        <input type="text" placeholder="Lastname" required>
        <input type="email" placeholder="Email" required>
        <input type="password" placeholder="Password" required>
        <input type="password" placeholder="Confirm Password" required>
        <button type="submit">Submit</button>
      </form>
      <p>Already have an account? <a href="#">Signin</a></p>
    </div>
  </div>

</body>
</html>
