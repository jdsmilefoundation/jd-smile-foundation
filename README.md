<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Sidebar Layout</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      display: flex;
      min-height: 100vh;
    }

    /* Sidebar */
    .sidebar {
      width: 220px;
      background: #0077aa;
      color: #fff;
      display: flex;
      flex-direction: column;
      padding-top: 30px;
      position: fixed;
      height: 100%;
    }

    .sidebar h2 {
      text-align: center;
      margin-bottom: 30px;
    }

    .sidebar a {
      color: #fff;
      padding: 15px 20px;
      text-decoration: none;
      display: block;
    }

    .sidebar a:hover {
      background: #005577;
    }

    /* Page Content */
    .content {
      margin-left: 220px; /* same as sidebar width */
      padding: 30px;
      flex: 1;
    }

    @media screen and (max-width: 768px) {
      .sidebar {
        position: relative;
        width: 100%;
        height: auto;
      }
      .content {
        margin-left: 0;
      }
    }
  </style>
</head>
<body>

  <div class="sidebar">
    <h2>JD Smile</h2>
    <a href="#about">About</a>
    <a href="#work">Our Work</a>
    <a href="#plans">Future Plans</a>
    <a href="#join">Join Us</a>
    <a href="#contact">Contact</a>
  </div>

  <div class="content">
    <h1>Welcome to JD Smile Foundation</h1>
    <p>This is your main content area. Add your sections here as needed.</p>
    <h2 id="about">About</h2>
    <p>Write about JD Smile Foundation here...</p>

    <h2 id="work">Our Work</h2>
    <p>Describe your work here...</p>

    <h2 id="plans">Future Plans</h2>
    <p>Write your plans here...</p>

    <h2 id="join">Join Us</h2>
    <p>Add a form or instructions here...</p>

    <h2 id="contact">Contact</h2>
    <p>Provide your contact details here...</p>
  </div>

</body>
</html>
