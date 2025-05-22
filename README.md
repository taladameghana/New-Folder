# New-Folder
Module 1-Bootstrap 5
1. Setting Up Bootstrap 5
Exercise 1.1:
Create a basic HTML page and link Bootstrap 5 via CDN.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Bootstrap 5 CDN Example</title>
  <!-- Bootstrap 5 CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>
  <div class="container mt-5">
    <h1 class="text-primary">Hello, Bootstrap 5!</h1>
    <p>This is a simple example using Bootstrap 5 via CDN.</p>
  </div>

  <!-- Bootstrap 5 JS Bundle (includes Popper) -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>

Exercise 1.2:
Set up a project using npm or downloaded Bootstrap files. Use the downloaded files in a sample
HTML page.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Bootstrap 5 Local Example</title>
  <!-- Bootstrap 5 CSS -->
  <link rel="stylesheet" href="css/bootstrap.min.css">
</head>
<body>
  <div class="container mt-5">
    <h1 class="text-success">Hello, Bootstrap 5!</h1>
    <p>This is a simple example using Bootstrap 5 locally.</p>
  </div>

  <!-- Bootstrap 5 JS Bundle -->
  <script src="js/bootstrap.bundle.min.js"></script>
</body>
</html>
2. Bootstrap Structure and Files
Exercise 2.1:
Explore the structure of the downloaded Bootstrap directory. Identify and explain the purpose of
the CSS, JS, and icons folders.
bootstrap/
├── css/
│   ├── bootstrap.css
│   ├── bootstrap.min.css
│   └── ...
├── js/
│   ├── bootstrap.bundle.js
│   ├── bootstrap.bundle.min.js
│   └── ...
└── icons/
    ├── bootstrap-icons.css
    └── ...

Exercise 2.2:
Modify your HTML to include Bootstrap's JavaScript plugins via bootstrap.bundle.min.js.
<head>
  <!-- Bootstrap CSS -->
  <link rel="stylesheet" href="css/bootstrap.min.css">
</head>
<body>
  <!-- Your content here -->

  <!-- Bootstrap JS Bundle -->
  <script src="js/bootstrap.bundle.min.js"></script>
</body>
3. Fundamentals of Responsive Grid Layout
Exercise 3.1:
Create a container with three columns that stack vertically on mobile, two-per-row on tablets,
and three-per-row on desktops.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Responsive Grid Example</title>
  <!-- Bootstrap 5 CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>
  <div class="container mt-4">
    <div class="row">
      <div class="col-12 col-md-6 col-lg-4 mb-4">
        <div class="p-3 border bg-light text-center">Column 1</div>
      </div>
      <div class="col-12 col-md-6 col-lg-4 mb-4">
        <div class="p-3 border bg-light text-center">Column 2</div>
      </div>
      <div class="col-12 col-md-6 col-lg-4 mb-4">
        <div class="p-3 border bg-light text-center">Column 3</div>
      </div>
    </div>
  </div>

  <!-- Bootstrap 5 JS Bundle -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>

Exercise 3.2:
Use .container, .row, and .col-* classes appropriately for responsive design.
<div class="container">
  <div class="row">
    <div class="col-12 col-md-6 col-lg-4">
      <!-- Content for Column 1 -->
    </div>
    <div class="col-12 col-md-6 col-lg-4">
      <!-- Content for Column 2 -->
    </div>
    <div class="col-12 col-md-6 col-lg-4">
      <!-- Content for Column 3 -->
    </div>
  </div>
</div>
4. Column Layouts and Grid Classes
Exercise 4.1:
Design a two-column layout with a sidebar (col-md-3) and content area (col-md-9).
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Two-Column Layout</title>
  <!-- Bootstrap 5 CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>
  <div class="container mt-4">
    <div class="row">
      <!-- Sidebar -->
      <div class="col-md-3 bg-light border p-3">
        <h4>Sidebar</h4>
        <p>Sidebar content goes here.</p>
      </div>
      <!-- Main Content -->
      <div class="col-md-9 bg-white border p-3">
        <h4>Main Content</h4>
        <p>Main content goes here.</p>
      </div>
    </div>
  </div>

  <!-- Bootstrap 5 JS Bundle -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>

Exercise 4.2:
Create a four-column layout (col-sm-3) with equal width.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Four-Column Layout</title>
  <!-- Bootstrap 5 CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>
  <div class="container mt-4">
    <div class="row">
      <div class="col-sm-3 bg-light border p-3 text-center">Column 1</div>
      <div class="col-sm-3 bg-light border p-3 text-center">Column 2</div>
      <div class="col-sm-3 bg-light border p-3 text-center">Column 3</div>
      <div class="col-sm-3 bg-light border p-3 text-center">Column 4</div>
    </div>
  </div>

  <!-- Bootstrap 5 JS Bundle -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
5. Alignment and Reordering in Grid
Exercise 5.1:
Use justify-content-center and align-items-center to center content inside a row.
<div class="container" style="height: 300px;">
  <div class="row d-flex justify-content-center align-items-center h-100">
    <div class="col-6 text-center">
      <div class="p-4 bg-light border">
        <p>This content is centered both horizontally and vertically.</p>
      </div>
    </div>
  </div>
</div>

Exercise 5.2:
Reorder columns on different screen sizes using order-md-2, order-md-1.
<div class="container">
  <div class="row">
    <div class="col-md-6 order-md-2 bg-light p-3">
      <h5>Second Column (appears first on small screens)</h5>
      <p>Content for the second column.</p>
    </div>
    <div class="col-md-6 order-md-1 bg-white p-3">
      <h5>First Column (appears second on small screens)</h5>
      <p>Content for the first column.</p>
    </div>
  </div>
</div>
6. Responsive Flexbox Utilities
Exercise 7.1:
Create a navbar using d-flex, flex-column, and flex-md-row for responsive behavior.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Responsive Navbar</title>
  <!-- Bootstrap 5 CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>
  <nav class="navbar bg-light">
    <div class="container d-flex flex-column flex-md-row align-items-center justify-content-between">
      <a class="navbar-brand mb-2 mb-md-0" href="#">Brand</a>
      <ul class="nav">
        <li class="nav-item">
          <a class="nav-link active" href="#">Home</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Features</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Pricing</a>
        </li>
      </ul>
    </div>
  </nav:contentReference[oaicite:5]{index=5}

Exercise 7.2:
Use justify-content-between and align-items-center in a card layout.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Card Layout</title>
  <!-- Bootstrap 5 CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>
  <div class="container mt-4">
    <div class="card p-3">
      <div class="d-flex justify-content-between align-items-center">
        <div>
          <h5 class="card-title mb-0">Card Title</h5>
          <small class="text-muted">Subtitle</small>
        </div>
        <button class="btn btn-primary">Action</button>
      </div>
    </div>
  </div>

  <!-- Bootstrap 5 JS Bundle -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
7. Typography
Exercise 7.1:
Create a sample page with different Bootstrap typography utilities: display-1, lead, text-muted,
fw-bold, etc.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Bootstrap Typography Example</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="p-4">

  <h1 class="display-1">Display 1 Heading</h1>
  <p class="lead">This is a lead paragraph. It stands out from regular paragraphs.</p>
  <p class="text-muted">This text is muted, making it less prominent.</p>
  <p class="fw-bold">This text is bold using the <code>.fw-bold</code> class.</p>
  <p class="fst-italic">This text is italicized using the <code>.fst-italic</code> class.</p>
  <p class="text-decoration-underline">This text is underlined using the <code>.text-decoration-underline</code> class.<

Exercise 7.2:
Use text-uppercase, text-lowercase, text-capitalize.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Bootstrap Text Transform Example</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="p-4">

  <p class="text-uppercase">this text is transformed to uppercase.</p>
  <p class="text-lowercase">THIS TEXT IS TRANSFORMED TO LOWERCASE.</p>
  <p class="text-capitalize">this text is transformed to capitalized form.</p>

</body>
</html>
8. Forms
Exercise 8.1:
Create a registration form using Bootstrap form components like form-control, form-check, and
input-group.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Bootstrap Registration Form</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="p-4">

  <div class="container">
    <h2 class="mb-4">Register</h2>
    <form>
      <div class="mb-3">
        <label for="fullName" class="form-label">Full Name</label>
        <input type="text" class="form-control" id="fullName" placeholder="Enter your full name">
      </div>

      <div class="mb-3">
        <label for="email" class="form-label">Email address</label>
        <div class="input-group">
          <span class="input-group-text">@</span>
          <input type="email" class="form-control" id="email" placeholder="Enter your email">
        </div>
      </div>

      <div class="mb-3">
        <label for="password" class="form-label">Password</label>
        <input type="password" class="form-control" id="password" placeholder="Enter your password">
      </div>

      <div class="mb-3 form-check">
        <input t

Exercise 8.2:
Style a login form using form-floating
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Bootstrap Login Form</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="p-4">

  <div class="container">
    <h2 class="mb-4">Login</h2>
    <form>
      <div class="form-floating mb-3">
        <input type="email" class="form-control" id="loginEmail" placeholder="name@example.com">
        <label for="loginEmail">Email address</label>
      </div>

      <div class="form-floating mb-3">
        <input type="password" class="form-control" id="loginPassword" placeholder="Password">
        <label for="loginPassword">Password</label>
      </div>

      <button type="submit" class="btn btn-primary">Login</button>
    </form>
  </div>

</body>
</html>
9. Buttons
Exercise 9.1:
Create buttons using all contextual classes: btn-primary, btn-secondary, btn-outline-*, etc.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Bootstrap Buttons Example</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="p-4">

  <h2>Solid Buttons</h2>
  <button type="button" class="btn btn-primary">Primary</button>
  <button type="button" class="btn btn-secondary">Secondary</button>
  <button type="button" class="btn btn-success">Success</button>
  <button type="button" class="btn btn-danger">Danger</button>
  <button type="button" class="btn btn-warning">Warning</button>
  <button type="button" class="btn btn-info">Info</button>
  <button type="button" class="btn btn-light">Light</button>
  <button type="button" class="btn btn-dark">Dark</button>
  <button type="button" class="btn btn-link">Link</button>

  <h2 class="mt-4">Outline Buttons</h2>
  <button type="button" class="btn btn-outline-primary">Primary</button>
  <button type="button" class="btn btn-outline-secondary">Secondary</button>
  <button type="button" class="btn btn-outline-success">Success</button>
  <button type="button" class="btn btn-outline-danger">Danger

Exercise 9.2:
Add button groups using btn-group, and create toggle buttons with checkboxes
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Bootstrap Button Groups</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="p-4">

  <h2>Button Group</h2>
  <div class="btn-group" role="group" aria-label="Basic example">
    <button type="button" class="btn btn-primary">Left</button>
    <button type="button" class="btn btn-primary">Middle</button>
    <button type="button" class="btn btn-primary">Right</button>
  </div>

  <h2 class="mt-4">Checkbox Toggle Buttons</h2>
  <div class="btn-group" role="group" aria-label="Checkbox toggle button group">
    <input type="checkbox" class="btn-check" id="btncheck1" autocomplete="off">
    <label class="btn btn-outline-primary" for="btncheck1">Checkbox 1</label>

    <input type="checkbox" class="btn-check" id="btncheck2" autocomplete="off">
    <label class="btn btn-outline-primary" for="btncheck2">Checkbox 2</label>

    <input type="checkbox" class="btn-check" id="btncheck3" autocomplete="off">
    <label class="btn btn-outline-primary" for="btncheck3">Checkbox 3</label>
  </div>

</body>
</html>
10. Navbars and Navigation
Exercise 10.1:
Create a responsive navbar with logo, navigation links, and a search form.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Responsive Navbar</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">Logo</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <a class="nav-link active" href="#">Home</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Features</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Pricing</a>
          </li>
        </ul>
        <form class="d-flex" role="search">
          <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
          <button

Exercise 10.2:
Use nav, nav-tabs, nav-pills for creating tabbed navigation.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Tabbed Navigation</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

  <!-- Nav Tabs -->
  <ul class="nav nav-tabs" id="myTab" role="tablist">
    <li class="nav-item" role="presentation">
      <a class="nav-link active" id="home-tab" data-bs-toggle="tab" href="#home" role="tab" aria-controls="home" aria-selected="true">Home</a>
    </li>
    <li class="nav-item" role="presentation">
      <a class="nav-link" id="profile-tab" data-bs-toggle="tab" href="#profile" role="tab" aria-controls="profile" aria-selected="false">Profile</a>
    </li>
    <li class="nav-item" role="presentation">
      <a class="nav-link" id="contact-tab" data-bs-toggle="tab" href="#contact" role="tab" aria-controls="contact" aria-selected="false">Contact</a>
    </li>
  </ul>
  <div class="tab-content" id="myTabContent">
    <div class="tab-pane fade show active" id="home" role="tabpanel" aria-labelledby="home-tab">Home content...</div>
    <div class="tab-pane fade" id="profile" role="tabpanel" aria-labelledby="profile-tab">Profile content...</div>
    <div class="tab-pane fade" id="contact" role="tabpanel" aria-labelledby="contact-tab">Contact content...</div>
  </div>

  <!-- Nav Pills -->
  <ul class="nav nav-pills">
    <li class="nav-item">
      <a class="nav-link active" id="pills-home-tab" data-bs-toggle="pill" href="#pills-home" role="tab" aria-controls="pills-home" aria-selected="true">Home</a>
    </li>
    <li class="nav-item">
      <a class="nav-link" id="pills-profile-tab" data-bs-toggle="pill" href="#pills-profile" role="tab" aria-controls="pills-profile" aria-selected="false">Profile</a>
    </li>
    <li class="nav-item">
      <a class="nav-link" id="pills-contact-tab" data-bs-toggle="pill" href="#pills-contact" role="tab" aria-controls="pills-contact" aria-selected="false">Contact</a>
    </li>
  </ul>
  <div class="tab-content">
    <div class="tab-pane fade show active" id="pills-home" role="tabpanel" aria-labelledby="pills-home-tab">Home content...</div>
    <div class="tab-pane fade" id="pills-profile" role="tabpanel" aria-labelledby="pills-profile-tab">Profile content...</div>
    <div class="tab-pane fade" id="pills-contact" role="tabpanel" aria-labelledby="pills-contact-tab">Contact content...</div>
  </div>

  <!-- Bootstrap JS and Popper.js -->
  <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.11.6/dist/umd/popper.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.min.js"></script>

</body>
</html>
11. Cards and Media Objects
Exercise 11.1:
Create a profile card using card, card-body, card-title, and card-img-top.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Profile Card</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="p-4">

  <div class="card" style="width: 18rem;">
    <img src="https://randomuser.me/api/portraits/men/14.jpg" class="card-img-top" alt="John Doe">
    <div class="card-body">
      <h5 class="card-title">John Doe</h5>
      <p class="card-text">Creative Designer passionate about crafting user-centric digital experiences.</p>
      <a href="#" class="btn btn-primary">Connect</a>
    </div>
  </div>

</body>
</html>

Exercise 11.2:
Design a media object layout using media and align an image to the left of the content.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Media Object</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="p-4">

  <div class="d-flex">
    <img src="https://randomuser.me/api/portraits/men/14.jpg" class="me-3 rounded-circle" alt="John Doe" style="width: 60px; height: 60px;">
    <div>
      <h5 class="fw-bold">John Doe</h5>
      <p class="mb-1">Creative Designer passionate about crafting user-centric digital experiences.</p>
      <small class="text-muted">Posted on February 19, 2021</small>
    </div>
  </div>

</body>
</html>
12. Spacing Utilities
Exercise 12.1:
Apply margin (m-3, mt-4) and padding (p-2, py-5) utilities on layout sections.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Spacing Utilities Example</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

  <div class="container mt-4">
    <section class="bg-light p-3 mb-4">
      <h2 class="mb-3">Section 1</h2>
      <p>This section has padding and margin applied using Bootstrap's spacing utilities.</p>
    </section>

    <section class="bg-secondary text-white p-2 py-5">
      <h2 class="mb-3">Section 2</h2>
      <p>Notice the larger vertical padding applied here.</p>
    </section>
  </div>

</body>
</html>

Exercise 12.2:
Build a pricing section where spacing improves the layout.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Pricing Section</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

  <div class="container py-5">
    <div class="row row-cols-1 row-cols-md-3 g-4">
      <div class="col">
        <div class="card shadow-sm">
          <div class="card-body">
            <h5 class="card-title">Free</h5>
            <p class="card-text">$0/month</p>
            <ul class="list-unstyled">
              <li>10 users included</li>
              <li>2 GB of storage</li>
              <li>Email support</li>
            </ul>
            <a href="#" class="btn btn-primary">Sign up</a>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card shadow-sm">
          <div class="card-body">
            <h5 class="card-title">Pro</h5>
            <p class="card-text">$15/month</p>
            <ul class="list-unstyled">
              <li>20 users included</li>
              <li>10 GB of storage</li>
              <li>Priority email support</li>
            </ul>
            <a href="#" class="btn btn-primary">Get started</a>
          </div>
        </div>
      </div>
      <div class="col">
        <div class="card shadow-sm">
          <div class="card-body">
            <h5 class="card-title">Enterprise</h5>
            <p class="card-text">$29/month</p>
            <ul class="list-unstyled">
              <li>30 users included</li>
              <li>15 GB of storage</li>
              <li>Phone and email support</li>
            </ul>
            <a href="#" class="btn btn-primary">Contact us</a>
          </div>
        </div>
      </div>
    </div>
  </div>

</body>
</html>
13. Colors and Backgrounds
Exercise 13.1:
Create a dashboard page using contextual background classes (bg-primary, bg-warning, etc.) and
text colors.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Dashboard</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

  <div class="container mt-4">
    <div class="row">
      <div class="col-md-4">
        <div class="p-4 mb-3 bg-primary text-white rounded">
          <h5>Sales</h5>
          <p>Monthly sales data and trends.</p>
        </div>
      </div>
      <div class="col-md-4">
        <div class="p-4 mb-3 bg-warning text-dark rounded">
          <h5>Alerts</h5>
          <p>Recent system alerts and notifications.</p>
        </div>
      </div>
      <div class="col-md-4">
        <div class="p-4 mb-3 bg-info text-white rounded">
          <h5>Updates</h5>
          <p>Latest updates and news.</p>
        </div>
      </div>
    </div>
  </div>

</body>
</html>

Exercise 13.2:
Use bg-gradient with bg-dark and white text.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Gradient Background</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

  <div class="container mt-4">
    <div class="p-5 bg-dark bg-gradient text-white rounded">
      <h2>Welcome to the Dashboard</h2>
      <p>Your personalized overview of the system's performance.</p>
    </div>
  </div>

</body>
</html>
14. Display and Visibility
Exercise 14.1:
Use d-none, d-md-block, d-lg-flex to hide/show sections based on screen size.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Responsive Display</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

  <div class="container mt-4">
    <div class="row">
      <div class="col-12">
        <div class="d-none d-md-block p-3 mb-3 bg-primary text-white">
          Visible on medium screens and larger
        </div>
        <div class="d-none d-lg-flex p-3 mb-3 bg-success text-white">
          Visible on large screens and larger
        </div>
        <div class="d-block d-md-none p-3 mb-3 bg-danger text-white">
          Visible on small screens only
        </div>
      </div>
    </div>
  </div>

</body>
</html>

Exercise 14.2:
Create a responsive sidebar that only shows on tablets and above.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Responsive Sidebar</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

  <div class="container-fluid">
    <div class="row">
      <!-- Sidebar -->
      <nav class="col-md-3 col-lg-2 d-none d-md-block bg-light sidebar">
        <div class="position-sticky">
          <ul class="nav flex-column">
            <li class="nav-item">
              <a class="nav-link active" href="#">
                Dashboard
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                Orders
              </a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                Products
              </a>
            </li>
          </ul>
        </div>
      </nav>

      <!-- Main content -->
      <main class="col-md-9 ms-sm-auto col-lg-10 px-4">
        <h2>Main Content</h2>
        <p>This is the main content area.</p>
      </main>
    </div>
  </div>

</body>
</html>
15. Borders, Shadows, and Rounded Corners
Exercise 15.1:
Add border utilities like border, border-primary, border-3, and rounded-circle to an image.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Styled Image</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="bg-light text-center p-4">

  <img src="https://via.placeholder.com/150" class="border border-primary border-3 rounded-circle" alt="Styled Image">

</body>
</html>

Exercise 15.2:
Use shadow, shadow-lg and rounded-pill in a card.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Card with Shadow</title>
  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="bg-light p-4">

  <div class="card shadow-lg rounded-pill" style="width: 18rem;">
    <img src="https://via.placeholder.com/150" class="card-img-top rounded-top" alt="Card image">
    <div class="card-body">
      <h5 class="card-title">Card Title</h5>
      <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
      <a href="#" class="btn btn-primary">Go somewhere</a>
    </div>
  </div>

</body>
</html>
16. Positioning Utilities
Exercise 16.1:
Create a fixed footer using position-fixed bottom-0.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Fixed Footer</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="min-vh-100 d-flex flex-column">

  <div class="container my-auto">
    <h1 class="text-center">Main Content</h1>
    <p class="text-center">Add your content here.</p>
  </div>

  <footer class="position-fixed bottom-0 start-0 end-0 bg-dark text-white text-center py-2">
    <p class="mb-0">© 2025 Your Company</p>:contentReference[oaicite:13]{index=13}:contentReference[oaicite:16]{index=16}

Exercise 16.2:
Use position-relative and position-absolute to overlay a badge over an image
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Image with Badge</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

  <div class="position-relative d-inline-block">
    <img src="https://via.placeholder.com/300" class="img-fluid" alt="Sample Image">
    <span class="position-absolute top-0 start-100 translate-middle badge rounded-pill bg-danger">
      New
    </span>
  </div>

</body>
</html>
17. Icons with Bootstrap Icons
Exercise 17.1:
Install and use Bootstrap Icons in a webpage: add social media icons in the footer.
<link href="https://cdn.jsdelivr.net/npm/bootstrap-icons/font/bootstrap-icons.css" rel="stylesheet">
<footer class="text-center text-white" style="background-color: #f1f1f1;">
  <div class="container pt-4">
    <section class="mb-4">
      <a href="#" class="btn btn-link btn-floating btn-lg text-dark m-1" role="button">
        <i class="bi bi-facebook"></i>
      </a>
      <a href="#" class="btn btn-link btn-floating btn-lg text-dark m-1" role="button">
        <i class="bi bi-twitter"></i>
      </a>
      <a href="#" class="btn btn-link btn-floating btn-lg text-dark m-1" role="button">
        <i class="bi bi-instagram"></i>
      </a>
      <a href="#" class="btn btn-link btn-floating btn-lg text-dark m-1" role="button">
        <i class="bi bi-linkedin"></i>
      </a>
    </section>
  </div>
</footer>

Exercise 17.2:
Replace text buttons with icon-only buttons using Bootstrap Icons.
<link href="https://cdn.jsdelivr.net/npm/bootstrap-icons/font/bootstrap-icons.css" rel="stylesheet">
<button type="button" class="btn btn-primary">
  <i class="bi bi-house-door"></i>
</button>
<button type="button" class="btn btn-secondary">
  <i class="bi bi-search"></i>
</button>
<button type="button" class="btn btn-danger">
  <i class="bi bi-trash"></i>
</button>
18. Bootstrap 5 JavaScript Plugins
Exercise 18.1:
Add a modal popup triggered by a button.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Modal Example</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

  <!-- Button to trigger modal -->
  <button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#exampleModal">
    Open Modal
  </button>

  <!-- Modal -->
  <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
    <div class="modal-dialog">
      <div class="modal-content">
        <div class="modal-header">
          <h5 class="modal-title" id="exampleModalLabel">Modal Title</h5>
          <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
        </div>
        <div class="modal-body">
          This is a simple modal example.
        </div>
        <div class="modal-footer">
          <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
          <button type="button" class="btn btn-primary">Save changes</button>
        </div>
      </div>
    </div>
  </div>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle:contentReference[oaicite:5]{index=5}

Exercise 18.2:
Create a collapsible accordion using accordion and Bootstrap JavaScript behavior.
         <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Accordion Example</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

  <div class="accordion" id="accordionExample">
    <div class="accordion-item">
      <h2 class="accordion-header" id="headingOne">
        <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
          Accordion Item #1
        </button>
      </h2>
      <div id="collapseOne" class="accordion-collapse collapse show" aria-labelledby="headingOne" data-bs-parent="#accordionExample">
        <div class="accordion-body">
          This is the first item's accordion body. It is shown by default, until the collapse plugin adds the appropriate classes that we use to style each element.
        </div>
      </div>
    </div>
    <div class="accordion-item">
      <h2 class="accordion-header" id="headingTwo">
        <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
          Accordion Item #2
        </button>
      </h2>
      <div id="collapseTwo" class="accordion-collapse collapse" aria-labelledby="headingTwo" data-bs-parent="#accordionExample">
        <div class="accordion-body">
          This is the second item's accordion body. It is hidden by default, until the collapse plugin adds the appropriate classes that we use to style each element.
        </div>
      </div>
    </div>
    <div class="accordion-item">
      <h2 class="accordion-header" id="headingThree">
        <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
          Accordion Item #3
        </button>
      </h2>
      <div id="collapseThree" class="accordion-collapse collapse" aria-labelledby="headingThree" data-bs-parent="#accordionExample">
        <div class="accordion-body">
          This is the third item's accordion body. It is hidden by default, until the collapse plugin adds the appropriate classes that we use to style each element.
        </div>
      </div>
    </div>
  </div>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
19. Customization with Sass
Exercise 19.1:
Set up a Bootstrap 5 project with Sass using npm.
mkdir my-bootstrap-project
cd my-bootstrap-project
npm init -y
npm install bootstrap sass --save-dev
my-bootstrap-project/
├── scss/
│   └── custom.scss
└── node_modules/
    └── bootstrap/
        ├── scss/
        └── js/
npx sass scss/custom.scss dist/styles.css
npm run build-css
npx sass --watch scss/custom.scss:dist/styles.css

Exercise 19.2:
Customize primary colors and border radius via _variables.scss and recompile Bootstrap.
// _variables.scss
$primary: #ff5733; // Custom primary color
$border-radius: 0.375rem; // Custom border radius
// custom.scss
@import "../node_modules/bootstrap/scss/functions";
@import "../node_modules/bootstrap/scss/variables";
@import "../node_modules/bootstrap/scss/mixins";
@import "../node_modules/bootstrap/scss/bootstrap";
Module 1-CSS3 Exercises
Theme: Styling the "Local Community Event Portal"
1. Why CSS? Inline vs. Internal vs. External
Scenario: The designer wants you to experiment with different ways to apply styles.
Objective: Understand various CSS inclusion methods and their impact.
Task:
• Apply an inline style to make one heading red.
• Use an embedded <style> tag in the <head> to define body background.
• Link an external stylesheet styles.css and move all reusable styles there.
• Add comments in your CSS to label each section (/* Header styles */)
1. Inline CSS
Usage: Applied directly within an HTML element using the style attribute.

Scope: Affects only the specific element it's applied to.

When to Use: Ideal for quick, one-off styling changes.


2. Internal CSS
Usage: Defined within a <style> tag in the <head> section of an HTML document.

Scope: Affects all elements within the same HTML document.

When to Use: Suitable for single-page documents or when styles are unique to that page.

3. External CSS
Usage: Stored in a separate .css file and linked to the HTML document using the <link> tag.

Scope: Affects multiple HTML documents that link to the same CSS file.

When to Use: Best for multi-page websites to maintain consistent styling across all pages.
Practical Example
HTML File (index.html)
html
Copy
Edit
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Styling Methods</title>
    <!-- Internal CSS -->
    <style>
        /* Body Background */
        body {
            background-color: #f0f0f0;
        }
    </style>
    <!-- External CSS -->
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <!-- Inline CSS -->
    <h1 style="color: red;">Welcome to CSS Styling</h1>
    <p>This is a demonstration of different CSS methods.</p>
</body>
</html>
External CSS File (styles.css)
css
Copy
Edit
/* Header Styles */
h1 {
    font-family: 'Arial', sans-serif;
    font-size: 2em;
    text-align: center;
}

/* Paragraph Styles */
p {
    font-family: 'Verdana', sans-serif;
    font-size: 1.2em;
    color: #333;
}
2. CSS Syntax and Comments
Scenario: You’ve joined a team and need to understand and maintain a large stylesheet.
Objective: Write clean, readable CSS with proper structure and comments.
Task:
• Create a section in styles.css with formatted rules and consistent indentation.
• Add descriptive comments above selectors.
• Example:
/* Style for main CTA button */
.cta-button {
 background-color: #007BFF;
 color: white;
}
/* ========================================================================
   Header Styles
   ======================================================================== */

/* Style for main navigation bar */
#navbar {
  background-color: #333; /* Dark background for contrast */
  padding: 10px 20px;      /* Adequate padding for spacing */
  text-align: center;      /* Center-align text */
}

/* Style for navigation links */
#navbar a {
  color: white;            /* White text color */
  padding: 14px 20px;      /* Padding for clickable area */
  text-decoration: none;   /* Remove underline */
  display: inline-block;   /* Align links horizontally */
}

#navbar a:hover {
  background-color: #ddd;  /* Light background on hover */
  color: black;            /* Dark text on hover */
}

/* ========================================================================
   Main Content Styles
   ======================================================================== */

/* Style for main content area */
.main-content {
  margin: 20px auto;       /* Center-align with margin */
  max-width: 1200px;       /* Maximum width for readability */
  padding: 20px;           /* Padding inside content */
}

/* Style for article sections */
.main-content article {
  margin-bottom: 30px;     /* Space between articles */
  border-bottom: 1px solid #ccc; /* Light border for separation */
  padding-bottom: 20px;    /* Padding inside article */
}

/* ========================================================================
   Footer Styles
   ======================================================================== */

/* Style for footer */
footer {
  background-color: #333; /* Dark background to match header */
  color: white;           /* White text color */
  text-align: center;     /* Center-align text */
  padding: 10px 0;        /* Padding for spacing */
  position: fixed;        /* Fixed at bottom */
  bottom: 0;              /* Align at bottom */
  width: 100%;            /* Full width */
}

3. Selectors Playground
Scenario: You need to style various elements based on IDs, classes, and element types.
Objective: Master different selector types.
Task:
• Use:
o Universal selector * to reset margin/padding
o Element selector to style all <h2>
o ID selector #mainHeader for the banner
o Class selector .eventCard for event containers
o Grouping selector for h3, p to style together
/* Reset margin and padding for all elements */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box; /* Ensures padding and borders are included in element's total width and height */
}
/* Style for all <h2> elements */
h2 {
  font-size: 2rem;
  color: #333;
  margin-bottom: 1rem;
}
/* Style for the element with id="mainHeader" */
#mainHeader {
  background-color: #007BFF;
  color: white;
  padding: 20px;
  text-align: center;
}
/* Style for all elements with class="eventCard" */
.eventCard {
  border: 1px solid #ccc;
  border-radius: 8px;
  padding: 15px;
  margin-bottom: 20px;
  background-color: #f9f9f9;
}
/* Style for <h3> and <p> elements */
h3, p {
  font-family: 'Arial', sans-serif;
  line-height: 1.6;
  color: #555;
}
/* ========================================================================
   Global Reset
   ======================================================================== */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* ========================================================================
   Header Styles
   ======================================================================== */
#mainHeader {
  background-color: #007BFF;
  color: white;
  padding: 20px;
  text-align: center;
}

/* ========================================================================
   Event Card Styles
   ======================================================================== */
.eventCard {
  border: 1px solid #ccc;
  border-radius: 8px;
  padding: 15px;
  margin-bottom: 20px;
  background-color: #f9f9f9;
}

/* ========================================================================
   Typography Styles
   ======================================================================== */
h2 {
  font-size: 2rem;
  color: #333;
  margin-bottom: 1rem;
}

h3, p {
  font-family: 'Arial', sans-serif;
  line-height: 1.6;
  color: #555;
}

4. Color & Background Styling
Scenario: You’re theming the portal based on a city council’s branding.
Objective: Apply consistent colors and background visuals.
Task:
• Use HEX and RGBA for setting text and background colors
• Add a background image to the body with fallback color
• Apply gradients to section headers using background: linear-gradient(...)
/* HEX color for text */
h1 {
  color: #2c3e50; /* Dark slate gray */
}

/* RGBA color for semi-transparent background */
section {
  background-color: rgba(46, 204, 113, 0.7); /* Semi-transparent green */
}
/* Body background with image and fallback color */
body {
  background-color: #ecf0f1; /* Light gray fallback */
  background-image: url('cityscape.jpg');
  background-size: cover;
  background-position: center;
}
/* Section header with linear gradient */
section header {
  background: linear-gradient(to right, #3498db, #8e44ad); /* Blue to purple */
  color: white;
  padding: 20px;
  text-align: center;
}

5. Typography: Fonts and Text
Scenario: The marketing team wants more appealing fonts and better readability.
Objective: Enhance textual appearance using CSS properties.
Task:
• Use @import or <link> to include a Google Font
• Set font-family, font-size, font-style, font-weight in different sections
• Use text-align, text-transform, letter-spacing, line-height on descriptions
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap">
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');
/* Body text */
body {
  font-family: 'Roboto', sans-serif;
  font-size: 16px;
  font-weight: 400;
  font-style: normal;
}

/* Main header */
h1 {
  font-family: 'Roboto', sans-serif;
  font-size: 2.5rem;
  font-weight: 700;
  font-style: normal;
}

/* Subheader */
h2 {
  font-family: 'Roboto', sans-serif;
  font-size: 2rem;
  font-weight: 700;
  font-style: italic;
}

/* Paragraph */
p {
  font-family: 'Roboto', sans-serif;
  font-size: 1rem;
  font-weight: 400;
  font-style: normal;
}
/* Paragraph styling */
p {
  text-align: justify;
  text-transform: capitalize;
  letter-spacing: 0.5px;
  line-height: 1.6;
}
<html>
<head>
  <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap">
  <style>
    /* Body text */
    body {
      font-family: 'Roboto', sans-serif;
      font-size: 16px;
      font-weight: 400;
      font-style: normal;
    }

    /* Main header */
    h1 {
      font-family: 'Roboto', sans-serif;
      font-size: 2.5rem;
      font-weight: 700;
      font-style: normal;
    }

    /* Subheader */
    h2 {
      font-family: 'Roboto', sans-serif;
      font-size: 2rem;
      font-weight: 700;
      font-style: italic;
    }

    /* Paragraph */
    p {
      font-family: 'Roboto', sans-serif;
      font-size: 1rem;
      font-weight: 400;
      font-style: normal;
      text-align: justify;
      text-transform: capitalize;
      letter-spacing: 0.5px;
      line-height: 1.6;
    }
  </style>
</head>
<body>
  <h1>Welcome to the City Council Portal</h1>
  <h2>Upcoming Events</h2>
  <p>Join us for the annual city cleanup event this Saturday. Volunteers are welcome to participate and make a difference in our community.</p>
</body>
</html>

6. Link and List Styling
Scenario: The default blue links and bullet lists don’t match the design.
Objective: Customize links and lists.
Task:
• Style links with :link, :hover, :active, and :visited pseudo-classes
• Use list-style-type, list-style-position, and remove bullets from nav menus
• Add padding and margin to list items for spacing
/* Default state for unvisited links */
a:link {
  color: #0056b3; /* Blue */
  text-decoration: none;
  font-weight: normal;
}

/* Visited links */
a:visited {
  color: #800080; /* Purple */
}

/* On hover */
a:hover {
  color: #ff6347; /* Tomato */
  text-decoration: underline;
}

/* When active (clicked) */
a:active {
  color: #ff4500; /* OrangeRed */
}
/* Remove bullets and reset margin/padding */
ul {
  list-style-type: none;
  list-style-position: outside;
  margin: 0;
  padding: 0;
}

/* Add spacing between list items */
ul li {
  margin-bottom: 10px;
  padding-left: 20px; /* Optional: Adds indentation */
  position: relative;
}

/* Optional: Custom bullet using ::before pseudo-element */
ul li::before {
  content: '•';
  color: #007bff; /* Blue */
  position: absolute;
  left: 0;
  top: 0;
}
/* Remove default list styling */
nav ul {
  list-style: none;
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: space-around;
}

/* Style individual list items */
nav ul li {
  margin: 0 15px;
  padding: 10px 20px;
}

/* Style links within the navigation */
nav ul li a {
  color: #ffffff;
  text-decoration: none;
  font-weight: bold;
  text-transform: uppercase;
}

/* Hover effect for links */
nav ul li a:hover {
  color: #ffd700; /* Gold */
}

7. Table Styling
Scenario: The events admin table needs a cleaner look.
Objective: Format tables using CSS.
Task:
• Style table, th, and td with borders, padding, and background color
• Add zebra striping to rows using nth-child(even)
• Use border-collapse: collapse and text-align: center
table, th, td {
  border: 1px solid #ddd;
  padding: 8px;
  text-align: center;
  border-collapse: collapse;
}
tr:nth-child(even) {
  background-color: #f2f2f2;
}
th {
  background-color: #4CAF50;
  color: white;
  font-weight: bold;
}
td:first-child, th:first-child {
  background-color: #e7f7e7;
}

td:last-child, th:last-child {
  background-color: #e7f7e7;
}

8. Box Model & Layout Control
Scenario: Sections are cramped and need spacing.
Objective: Control element spacing with margin, padding, border, and outline.
Task:
• Use developer tools to inspect and tweak box model properties
• Add border, padding, and margin to .eventCard
• Add outline to highlight selected fields in a form
• Compare visibility: hidden vs. display: none
/* Global Box Model Reset */
*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

/* Body Styling */
body {
  font-family: 'Arial', sans-serif;
  line-height: 1.6;
  background-color: #f4f4f4;
  color: #333;
  padding: 20px;
}

/* Section Styling */
section {
  margin-bottom: 40px;
  padding: 20px;
  border: 1px solid #ddd;
  border-radius: 8px;
  background-color: white;
}

/* Event Card Styling */
.eventCard {
  margin: 20px 0;
  padding: 15px;
  border: 1px solid #ccc;
  border-radius: 8px;
  background-color: #fff;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}

/* Form Field Focus Outline */
input:focus,
textarea:focus,
select:focus {
  outline: 3px solid #007bff;
  outline-offset: 2px;
}

/* Visibility vs. Display */
.hidden-element {
  visibility: hidden; /* Element is invisible but still occupies space */
}

.removed-element {
  display: none; /* Element is removed from the layout */
}

9. Multiple Columns in Text
Scenario: The community bulletin needs to be displayed like a newspaper.
Objective: Use CSS3 multi-column layout.
Task:
• Create a news article section and apply:
column-count: 2;
column-gap: 30px;
column-rule: 1px solid gray;
/* News Article Section */
.news-article {
  column-count: 2;               /* Divide content into 2 columns */
  column-gap: 30px;              /* Set 30px gap between columns */
  column-rule: 1px solid gray;   /* Add a 1px solid gray line between columns */
  padding: 20px;                 /* Add padding inside the section */
  background-color: #fff;        /* Set background color to white */
  border-radius: 8px;            /* Rounded corners */
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1); /* Subtle shadow for depth */
  font-family: 'Georgia', serif; /* Use serif font for a newspaper feel */
  line-height: 1.6;              /* Improve readability */
}

10. Responsive Web Design with Media Queries
Scenario: Users will access the portal on phones, tablets, and desktops.
Objective: Apply media queries for responsiveness.
Task:
• Add a media query for screens smaller than 768px
• Stack navigation links vertically instead of horizontally
• Reduce image sizes and font sizes
• Use %, vw, vh for flexible layouts
• Bonus: Try Flexbox or Grid for responsive layouts
@media only screen and (max-width: 768px) {
  /* Styles for mobile and tablet devices */
}
@media only screen and (max-width: 768px) {
  nav ul {
    display: block;
    text-align: center;
  }

  nav ul li {
    display: block;
    margin: 10px 0;
  }
}
@media only screen and (max-width: 768px) {
  img {
    width: 100%;
    height: auto;
  }

  body {
    font-size: 14px;
  }
}
.container {
  width: 100%;
  padding: 5%;
}

.header {
  height: 10vh;
}
@media only screen and (max-width: 768px) {
  .flex-container {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .flex-item {
    width: 90%;
    margin: 10px 0;
  }
}

11. Debug and Test with Dev Tools and VS Code
Scenario: Some users report layout breaking on smaller screens.
Objective: Use DevTools to test styles and debug.
Task:
• Use Chrome’s device toolbar to simulate different screen sizes
• Inspect applied styles and test different values live
• Use the Network tab to check if the external CSS is loaded
🛠️ Debugging with Chrome DevTools
1. Simulate Different Screen Sizes
Open Chrome DevTools by pressing Ctrl + Shift + I (Windows/Linux) or Cmd + Option + I (Mac).

Click the Toggle Device Toolbar button or press Ctrl + Shift + M (Windows/Linux) or Cmd + Shift + M (Mac) to enter device emulation mode.
DevTools Tips
+1
Tutkit.com
+1

Use the Dimensions drop-down to select a specific device or enter custom width and height values. 
Chrome for Developers
+1
DebugBear
+1

To view media query breakpoints, click the More options (three dots) in the device toolbar and select Show media queries. 
Chrome for Developers
+1
DebugBear
+1

2. Inspect Applied Styles
In the Elements panel, select the element you want to inspect.
Chrome for Developers

In the Styles pane, review the applied CSS rules.

To test different values live, modify the CSS properties directly in the Styles pane.

3. Check if External CSS is Loaded
Go to the Network tab in DevTools.
web.dev
+1
Google Help
+1

Reload the page.

Look for your external CSS file (e.g., styles.css) in the list of network requests.

If the file is not listed, ensure that the <link> tag in your HTML file correctly references the CSS file's path.

Testing Responsiveness in Visual Studio Code
1. Use Live Server Extension
Install the Live Server extension from the VS Code Marketplace.
Ritwick Dey

Right-click on your index.html file and select Open with Live Server.

This will launch a local development server and open your webpage in the browser.

As you make changes to your code, the browser will automatically refresh to reflect the updates.

2. Preview in Different Devices
While your page is open in the browser, use the browser's developer tools to simulate different devices and screen sizes, as described in the Chrome DevTools section above
Module 1-HTML 5
HTML5 Exercises
Project Theme: Local Community Event Portal
A local city council wants a lightweight, browser-based portal to help residents register for
events, check locations, and access basic services.
1. Create the HTML5 Base Template
Scenario: You’re setting up the base document that every page on the portal will use.
Objective: Ensure semantic structure and compatibility across browsers.
Task:
• Use <!DOCTYPE html>, <html lang="en">, <meta charset="UTF-8">
• Add comments to label sections like "Navigation", "Main", "Footer"
• Save as index.html and open it in Chrome
• Inspect the document structure in Chrome Dev Tools
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Local Community Event Portal</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>

  <!-- Navigation -->
  <nav>
    <ul>
      <li><a href="#home">Home</a></li>
      <li><a href="#events">Events</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <!-- Main Content -->
  <main id="home">
    <section id="events">
      <h2>Upcoming Events</h2>
      <!-- Event details go here -->
    </section>
    <section id="contact">
      <h2>Contact Us</h2>
      <!-- Contact form goes here -->
    </section>
  </main>

  <!-- Footer -->
  <footer>
    <p>&copy; 2025 Local Community Council</p>
  </footer>

</body>
</html>


2. Navigation and Linking
Scenario: Users should navigate between "Home", "Events", and "Contact" sections.
Objective: Provide intuitive navigation and section-based references.
Task:
• Use <nav> with anchor tags <a href="#events">Events</a>
• Define matching IDs for each section like <section id="events">
• Add a link to an external help document using <a href="help.html" target="_blank">
<nav>
  <ul>
    <li><a href="#home">Home</a></li>
    <li><a href="#events">Events</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="help.html" target="_blank">Help</a></li>
  </ul>
</nav>

3. Welcome Message with Styling and ID/Class
Scenario: Display a welcome banner styled uniquely for a logged-in user.
Objective: Practice block/inline tags and differentiate id and class
Task:
• Use <div id="welcomeBanner"> and apply a blue background via internal CSS
• Use inline styles for a special offer <span> (e.g., color red, bold)
• Apply the .highlight class to certain elements for visual emphasis
<div id="welcomeBanner">
  <h1>Welcome to the Local Community Event Portal</h1>
  <p>Explore upcoming events and connect with your community.</p>
</div>

<p>Special Offer: <span class="highlight">Register now and get a free community guide!</span></p>
4. Image Gallery for Community Events
Scenario: Show images from past events in a table layout.
Objective: Work with <img>, tables, and formatting tags.
Task:
• Use a <table> with 2 rows and 3 columns of <img> tags
• Include alt, title, and style each image with borders using a class
• Add a caption to describe each event
<table>
  <caption>Past Community Events</caption>
  <tr>
    <td><img src="event1.jpg" alt="Community Picnic" title="Community Picnic" class="event-img"></td>
    <td><img src="event2.jpg" alt="Charity Run" title="Charity Run" class="event-img"></td>
    <td><img src="event3.jpg" alt="Art Exhibition" title="Art Exhibition" class="event-img"></td>
  </tr>
  <tr>
    <td><img src="event4.jpg" alt="Food Drive" title="Food Drive" class="event-img"></td>
    <td><img src="event5.jpg" alt="Music Festival" title="Music Festival" class="event-img"></td>
    <td><img src="event6.jpg" alt="Community Clean-up" title="Community Clean-up" class="event-img"></td>
  </tr>
</table>
5. Event Registration Form
Scenario: Residents need to register for events.
Objective: Practice input types, validation, placeholder, autofocus, and output
Task:
• Include fields: name (text), email (email), date (date), event type (select), message
(textarea)
• Add placeholder, required, and autofocus
• Display a confirmation message using <output> when the form is submitted
• Style the form using CSS
<form id="registrationForm">
  <label for="name">Name:</label>
  <input type="text" id="name" name="name" placeholder="Your Name" required autofocus><br><br>

  <label for="email">Email:</label>
  <input type="email" id="email" name="email" placeholder="Your Email" required><br><br>

  <label for="eventType">Event Type:</label>
  <select id="eventType" name="eventType">
    <option value="workshop">Workshop</option>
    <option value="seminar">Seminar</option>
    <option value="webinar">Webinar</option>
  </select><br><br>

  <label for="message">Message:</label><br>
  <textarea id="message" name="message" rows="4" cols="50" placeholder="Your Message"></textarea><br><br>

  <input type="submit" value="Register">
</form>

<output id="confirmationMessage"></output>
6. Event Feedback with Events Handling
Scenario: Collect real-time feedback and interactions from the user.
Objective: Handle blur, change, click, double-click, and keyboard events.
Task:
• Use onblur to validate a phone number field
• Use onchange on a dropdown to display the selected event fee
• onclick on a submit button to show a confirmation
• ondblclick on an image to enlarge it
• Capture key events in the feedback textarea and count characters
<form id="feedbackForm">
  <label for="phone">Phone Number:</label>
  <input type="tel" id="phone" name="phone" onblur="validatePhone()"><br><br>

  <label for="eventFee">Event Fee:</label>
  <select id="eventFee" name="eventFee" onchange="displayFee()">
    <option value="free">Free</option>
    <option value="paid">Paid</option>
  </select><br><br>

  <label for="feedback">Feedback:</label><br>
  <textarea id="feedback" name="feedback" rows="4" cols="50" oninput="countCharacters()"></textarea><br><br>

  <input type="submit" value="Submit">
</form>

<p id="phoneValidation"></p>
<p id="feeDisplay"></p>
<p id="charCount">Characters: 0</p>
7. Video Invite with Media Events
Scenario: Show a short event promo video.
Objective: Work with <video> and oncanplay event
Task:
• Insert a <video> element with source and controls
• Use oncanplay to display a message like "Video ready to play"
• Use onbeforeunload to warn users if they try to leave the form page unfinished
<video id="promoVideo" width="320" height="240" controls oncanplay="videoReady()">
  <source src="promo.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

<script>
  function videoReady() {
    alert("Video is ready to play!");
  }
</script>
8. Saving User Preferences
Scenario: Store preferred event type for returning users.
Objective: Work with localStorage, sessionStorage, and deletion
Task:
• Save selected event type in localStorage
• On reload, retrieve and pre-select it
• Add a "Clear Preferences" button that clears both localStorage and sessionStorage
<select id="eventType" onchange="savePreference()">
  <option value="workshop">Workshop</option>
  <option value="seminar">Seminar</option>
  <option value="webinar">Webinar</option>
</select>

<button onclick="clearPreferences()">Clear Preferences</button>

<script>
  window.onload = function() {
    const savedPreference = localStorage.getItem('preferredEventType');
    if (savedPreference) {
      document.getElementById('eventType').value = savedPreference;
    }
  };

  function savePreference() {
    const selectedEventType = document.getElementById('eventType').value;
    localStorage.setItem('preferredEventType', selectedEventType);
  }

  function clearPreferences() {
    localStorage.removeItem('preferredEventType');
    sessionStorage.clear();
    alert("Preferences cleared!");
  }
</script>
9. Geolocation for Event Mapping
Scenario: Locate the nearest event to the user.
Objective: Practice geolocation.getCurrentPosition, error handling, and options
Task:
• Create a button “Find Nearby Events”
• On click, use getCurrentPosition to get and display coordinates
• Handle permission denial and timeouts
• Use high accuracy options

::contentReference[oaicite:138]{index=138}
 
10.Debugging with Chrome DevTools
Scenario: A few users report layout issues and script errors.
Objective: Use Chrome DevTools and VS Code features to debug.
Task:
• Use “Inspect Element” to modify styles and experiment live
• Use the Console tab to view logs from your <script>
• Add breakpoints in JS and reload the page to watch variable values
Debugging with Chrome DevTools
1. Inspect and Modify Styles Live
Open DevTools: Press Ctrl + Shift + I (Windows/Linux) or Cmd + Option + I (Mac).

Navigate to the Elements Panel: Here, you can select any element on your page to view and edit its HTML and CSS.

Edit Styles: In the Styles pane, modify CSS properties to see changes in real-time. This helps in adjusting margins, padding, colors, and more to fix layout issues.

2. Monitor JavaScript Errors
Access the Console Panel: Switch to the Console tab to view any JavaScript errors or warnings.

Log Outputs: Use console.log() in your scripts to output variable values and track the flow of execution.

Clear Console: Click the trash can icon to clear the console for fresh logs.
DEV Community

3. Set Breakpoints and Step Through Code
Open the Sources Panel: Locate your JavaScript file in the file navigator.

Add Breakpoints: Click on the line number where you want to pause execution.

Control Execution: Use the buttons to step over, step into, or resume script execution.

Inspect Variables: Check the Scope and Watch panels to view variable values and call stack.
DEV Community
+1
CoderPad
+1
HappyFox
+3
Buddy
+3
DEV Community
+3

🖥️ Debugging with Visual Studio Code
1. Set Up Browser Debugging
Install Chrome Debugger Extension: In VS Code, go to the Extensions view (Ctrl + Shift + X), search for "Debugger for Chrome," and install it.

Configure Launch Settings: Create a launch.json file in the .vscode folder with the following configuration:
Visual Studio Code

json
Copy
Edit
  {
    "version": "0.2.0",
    "configurations": [
      {
        "type": "chrome",
        "request": "launch",
        "name": "Launch Chrome against localhost",
        "url": "http://localhost:3000",
        "webRoot": "${workspaceFolder}"
      }
    ]
  }
Replace "http://localhost:3000" with the URL of your local development server.

2. Start Debugging
Launch Debugger: Press F5 or click on the green play button in the Run and Debug panel.

Set Breakpoints: Click on the gutter next to line numbers in your JavaScript files to set breakpoints.

Inspect Variables: Use the Variables and Watch panels to monitor variable values during execution.

Debug Console: View outputs and errors in the Debug Console.
Visual Studio Code
+3
Stack Overflow
+3
Zapier
+3

Practical Tips
Reproduce the Issue: Consistently reproduce the bug to understand its behavior.

Use Conditional Breakpoints: Right-click a breakpoint and select "Edit breakpoint" to add conditions, pausing execution only when specific criteria are met.

Monitor Network Requests: Use the Network panel to view API calls and responses, ensuring data is fetched correctly.

Check for Layout Shifts: Utilize the Performance panel to record and analyze layout shifts and rendering issues
Module 1 - Java Script
JavaScript Exercises
Project Theme: "Local Community Event Portal"
Users can view upcoming events, register, filter events by category or location, and interact
dynamically with the portal.
1. JavaScript Basics & Setup
Scenario: Set up your community portal to use JavaScript.
Objective: Configure environment and test basic script functionality.
Task:
• Use <script src="main.js"></script> in HTML
• Log "Welcome to the Community Portal" using console.log()
• Use an alert to notify when the page is fully loaded
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Community Event Portal</title>
    <!-- Link to external CSS file -->
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <!-- Navigation Section -->
    <nav>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#events">Events</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <!-- Main Content Section -->
    <main>
        <h1>Welcome to the Community Event Portal</h1>
        <p>Discover and register for upcoming events in your community.</p>
    </main>

    <!-- Footer Section -->
    <footer>
        <p>&copy; 2025 Community Event Portal</p>
    </footer>

    <!-- Link to external JavaScript file -->
    <script src="main.js"></script>
</body>
</html>
2. Create the JavaScript File// Log a welcome message to the console
console.log("Welcome to the Community Portal");

// Alert the user when the page is fully loaded
window.onload = function() {
    alert("Page is fully loaded!");
};
2. Syntax, Data Types, and Operators
Scenario: Store event details like name, date, and available seats.
Objective: Use proper data types and operations.
Task:
• Use const for event name and date, let for seats
• Concatenate event info using template literals
• Use ++ or -- to manage seat count on registration
// Event details
const eventName = "Community Cleanup";
const eventDate = "2025-06-15";
let availableSeats = 50;

// Display event information
console.log(`Event: ${eventName}`);
console.log(`Date: ${eventDate}`);
console.log(`Seats Available: ${availableSeats}`);

// Simulate a registration
availableSeats--; // Decrease seat count by 1
console.log(`Seats Available after registration: ${availableSeats}`);
3. Conditionals, Loops, and Error Handling
Scenario: Only show valid events and limit registrations.
Objective: Apply conditions and handle invalid data.
User Story: As a user, I want only upcoming events with seats to be displayed.
Task:
• Use if-else to hide past or full events
• Loop through the event list and display using forEach()
• Wrap registration logic in try-catch to handle errors
// Sample events data
const events = [
  { id: 1, name: "Community Yoga", date: "2025-06-15", seatsAvailable: 20 },
  { id: 2, name: "Art Workshop", date: "2025-05-10", seatsAvailable: 0 },
  { id: 3, name: "Cooking Class", date: "2025-07-20", seatsAvailable: 5 },
  { id: 4, name: "Music Concert", date: "2025-04-25", seatsAvailable: 15 }
];

// Function to check if an event is upcoming
function isUpcoming(eventDate) {
  const today = new Date();
  const eventDateObj = new Date(eventDate);
  return eventDateObj >= today;
}

// Function to register for an event
function registerForEvent(eventId) {
  try {
    const event = events.find(e => e.id === eventId);
    if (!event) throw new Error("Event not found.");
    if (!isUpcoming(event.date)) throw new Error("Event has already passed.");
    if (event.seatsAvailable <= 0) throw new Error("No seats available.");

    // Proceed with registration
    event.seatsAvailable--;
    console.log(`Successfully registered for ${event.name}. Remaining seats: ${event.seatsAvailable}`);
  } catch (error) {
    console.error(error.message);
  }
}

// Display upcoming events with available seats
events.forEach(event => {
  if (isUpcoming(event.date) && event.seatsAvailable > 0) {
    console.log(`${event.name} - Date: ${event.date} - Seats Available: ${event.seatsAvailable}`);
  }
});

// Example usage
registerForEvent(1); // Attempt to register for the first event
4. Functions, Scope, Closures, Higher-Order Functions
Scenario: Create reusable functions for event operations.
Objective: Encapsulate logic and use closures.
Task:
• Create addEvent(), registerUser(), filterEventsByCategory()
• Use closure to track total registrations for a category
• Pass callbacks to filter functions for dynamic search
function createEventCounter() {
  let count = 0;
  return function() {
    count++;
    console.log(`Event registrations: ${count}`);
  };
}

const registerEvent = createEventCounter();
registerEvent(); // Output: Event registrations: 1
registerEvent(); // Output: Event registrations: 2
5. Objects and Prototypes
Scenario: Each event is an object with properties and methods.
Objective: Model real-world entities using objects.
Task:
• Define Event constructor or class
• Add checkAvailability() to prototype
• List object keys and values using Object.entries()
function Event(name, date, seats) {
  this.name = name;
  this.date = new Date(date);
  this.seats = seats;
}

// Adding a method to the prototype
Event.prototype.checkAvailability = function() {
  return this.seats > 0 ? 'Seats available' : 'Sold out';
};
class Event {
  constructor(name, date, seats) {
    this.name = name;
    this.date = new Date(date);
    this.seats = seats;
  }

  checkAvailability() {
    return this.seats > 0 ? 'Seats available' : 'Sold out';
  }
}
const event = new Event('Community Picnic', '2025-06-15', 50);
console.log(Object.entries(event));
[
  ['name', 'Community Picnic'],
  ['date', '2025-06-15T00:00:00.000Z'],
  ['seats', 50]
]
6. Arrays and Methods
Scenario: Manage an array of all community events.
Objective: Use array methods for CRUD operations.
Task:
• Add new events using .push()
• Use .filter() to show only music events
• Use .map() to format display cards (e.g., "Workshop on Baking")
// Initial array of events
let events = [
  { name: "Art Workshop", category: "Art", date: "2025-06-10" },
  { name: "Music Concert", category: "Music", date: "2025-06-15" }
];

// 1. Add a new event using .push()
events.push({ name: "Baking Class", category: "Cooking", date: "2025-06-20" });

// 2. Filter events to show only those in the 'Music' category
let musicEvents = events.filter(event => event.category === "Music");

// 3. Format event display using .map()
let eventCards = events.map(event => `${event.name} - ${event.category} on ${event.date}`);

// Output the results
console.log("All Events:");
console.log(events);

console.log("\nMusic Events:");
console.log(musicEvents);

console.log("\nEvent Cards:");
console.log(eventCards);
7. DOM Manipulation
Scenario: Display all events dynamically on the webpage.
Objective: Render events using JS.
Task:
• Access DOM elements using querySelector()
• Create and append event cards using createElement()
• Update UI when user registers or cancels
// Sample array of event objects
const events = [
  { id: 1, name: "Art Workshop", category: "Art", date: "2025-06-10", seats: 10 },
  { id: 2, name: "Music Concert", category: "Music", date: "2025-06-15", seats: 0 },
  { id: 3, name: "Baking Class", category: "Cooking", date: "2025-06-20", seats: 5 }
];

// Access the container element
const container = document.querySelector('#event-container');

// Function to create and append event cards
function renderEvents() {
  // Clear existing content
  container.innerHTML = '';

  events.forEach(event => {
    // Create card element
    const card = document.createElement('div');
    card.classList.add('event-card');

    // Event details
    const title = document.createElement('h3');
    title.textContent = event.name;

    const category = document.createElement('p');
    category.textContent = `Category: ${event.category}`;

    const date = document.createElement('p');
    date.textContent = `Date: ${event.date}`;

    const seats = document.createElement('p');
    seats.textContent = `Available Seats: ${event.seats}`;

    // Register button
    const button = document.createElement('button');
    button.textContent = event.seats > 0 ? 'Register' : 'Sold Out';
    button.disabled = event.seats === 0;

    // Event listener for registration
    button.addEventListener('click', () => {
      if (event.seats > 0) {
        event.seats--;
        renderEvents(); // Re-render to update UI
      }
    });

    // Append elements to card
    card.appendChild(title);
    card.appendChild(category);
    card.appendChild(date);
    card.appendChild(seats);
    card.appendChild(button);

    // Append card to container
    container.appendChild(card);
  });
}

// Initial render
renderEvents();
8. Event Handling
Scenario: Add interactive elements like buttons and filters.
Objective: Respond to user actions.
Task:
• Use onclick for "Register" buttons
• Use onchange to filter events by category
• Use keydown to allow quick search by name
<input type="text" id="searchInput" placeholder="Search events by name" />
<select id="categoryFilter">
  <option value="">All Categories</option>
  <option value="Art">Art</option>
  <option value="Music">Music</option>
  <option value="Cooking">Cooking</option>
</select>
<div id="eventContainer"></div>
9. Async JS, Promises, Async/Await
Scenario: Fetch event data from a mock API.
Objective: Use asynchronous logic for remote operations.
Task:
• Fetch events from a mock JSON endpoint
• Use .then() and .catch() to handle results
• Rewrite using async/await and show loading spinner
const loader = document.getElementById('loader');
const container = document.getElementById('eventContainer');

function fetchEventsWithThen() {
  loader.style.display = 'block'; // Show loader
  fetch('https://jsonplaceholder.typicode.com/posts') // Mock API endpoint
    .then(response => {
      if (!response.ok) {
        throw new Error('Network response was not ok');
      }
      return response.json();
    })
    .then(events => {
      renderEvents(events);
    })
    .catch(error => {
      console.error('Fetch error:', error);
      container.innerHTML = '<p>Error loading events.</p>';
    })
    .finally(() => {
      loader.style.display = 'none'; // Hide loader
    });
}

function renderEvents(events) {
  container.innerHTML = ''; // Clear existing content
  events.slice(0, 5).forEach(event => {
    const card = document.createElement('div');
    card.classList.add('event-card');
    card.innerHTML = `
      <h3>${event.title}</h3>
      <p>${event.body}</p>
    `;
    container.appendChild(card);
  });
}

// Call the function
fetchEventsWithThen();
10. Modern JavaScript Features
Scenario: Refactor code to be concise and maintainable.
Objective: Use ES6+ features.
Task:
• Use let, const, default parameters in functions
• Use destructuring to extract event details
• Use spread operator to clone event list before filtering
// Sample array of event objects
const events = [
  { id: 1, name: "Art Workshop", category: "Art", date: "2025-06-10", seats: 10 },
  { id: 2, name: "Music Concert", category: "Music", date: "2025-06-15", seats: 5 },
  { id: 3, name: "Baking Class", category: "Cooking", date: "2025-06-20", seats: 8 }
];

// Function to render events
const renderEvents = (eventList = []) => {
  const container = document.querySelector('#eventContainer');
  container.innerHTML = ''; // Clear existing content

  eventList.forEach(({ id, name, category, date, seats }) => {
    const card = document.createElement('div');
    card.classList.add('event-card');

    card.innerHTML = `
      <h3>${name}</h3>
      <p>Category: ${category}</p>
      <p>Date: ${date}</p>
      <p>Available Seats: ${seats}</p>
      <button id="register-${id}" ${seats === 0 ? 'disabled' : ''}>
        ${seats > 0 ? 'Register' : 'Sold Out'}
      </button>
    `;

    container.appendChild(card);

    // Add event listener for registration
    const registerBtn = document.querySelector(`#register-${id}`);
    registerBtn.addEventListener('click', () => registerUser(id));
  });
};

// Function to register a user for an event
const registerUser = (eventId) => {
  const eventIndex = events.findIndex(event => event.id === eventId);
  if (eventIndex !=
11. Working with Forms
Scenario: Create a registration form for event sign-up.
Objective: Connect form inputs to JavaScript.
Task:
• Capture name, email, and selected event using form.elements
• Prevent default form behavior using event.preventDefault()
• Validate inputs and show errors inline
document.addEventListener('DOMContentLoaded', () => {
  const form = document.getElementById('registrationForm');

  form.addEventListener('submit', function (event) {
    event.preventDefault(); // Prevent form from submitting

    // Clear previous error messages
    clearErrors();

    // Retrieve form values
    const name = form.elements['name'].value.trim();
    const email = form.elements['email'].value.trim();
    const selectedEvent = form.elements['event'].value;

    let isValid = true;

    // Validate name
    if (name === '') {
      displayError('nameError', 'Name is required.');
      isValid = false;
    }

    // Validate email
    if (email === '') {
      displayError('emailError', 'Email is required.');
      isValid = false;
    } else if (!validateEmail(email)) {
      displayError('emailError', 'Please enter a valid email address.');
      isValid = false;
    }

    // Validate event selection
    if (selectedEvent === '') {
      displayError('eventError', 'Please select an event.');
      isValid = false;
    }

    if (isValid) {
      // Proceed with form submission or further processing
      alert('Registration successful!');
      form.reset();
    }
  });

  // Function to display error messages
  function displayError(elementId, message) {
    const errorElement = document.getElementById(elementId);
    if (errorElement) {
      errorElement.textContent = message;
    }
  }

  // Function to clear all error messages
  function clearErrors() {
    const errorElements = document.querySelectorAll('.error');
    errorElements.forEach((element) => {
      element.textContent = '';
    });
  }

  // Function to validate email format
  function validateEmail(email) {
    // Simple email regex for demonstration purposes
    const re = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
    return re.test(email);
  }
});
12. AJAX & Fetch API
Scenario: Send user registration to the server.
Objective: Simulate backend communication.
Task:
• Use fetch() to POST user data to a mock API
• Show success/failure message after submission
• Use setTimeout() to simulate a delayed response
document.addEventListener('DOMContentLoaded', () => {
  const form = document.getElementById('registrationForm');
  const messageDiv = document.getElementById('message');

  form.addEventListener('submit', function (event) {
    event.preventDefault(); // Prevent default form submission

    // Clear previous messages
    clearErrors();
    messageDiv.textContent = '';

    // Retrieve form values
    const name = form.elements['name'].value.trim();
    const email = form.elements['email'].value.trim();
    const selectedEvent = form.elements['event'].value;

    let isValid = true;

    // Validate name
    if (name === '') {
      displayError('nameError', 'Name is required.');
      isValid = false;
    }

    // Validate email
    if (email === '') {
      displayError('emailError', 'Email is required.');
      isValid = false;
    } else if (!validateEmail(email)) {
      displayError('emailError', 'Please enter a valid email address.');
      isValid = false;
    }

    // Validate event selection
    if (selectedEvent === '') {
      displayError('eventError', 'Please select an event.');
      isValid = false;
    }

    if (isValid) {
      // Simulate delayed response
      messageDiv.textContent = 'Submitting registration...';
      setTimeout(() => {
        // Send POST request to mock API
        fetch('https://jsonplaceholder.typicode.com/posts', {
          method: 'POST',
          headers: {
            'Content-Type': 'application/json'
          },
          body: JSON.stringify({ name, email, event: selectedEvent })
        })
          .then(response => {
            if (!response.ok) {
              throw new Error('Network response was not ok');
            }
            return response.json();
          })
          .then(data => {
            messageDiv.textContent = 'Registration successful!';
            form.reset();
          })
          .catch(error => {
            console.error('Fetch error:', error);
            messageDiv.textContent = 'Registration failed. Please try again.';
          });
      }, 2000); // 2-second delay
    }
  });

  // Function to display error messages
  function displayError(elementId, message) {
    const errorElement = document.getElementById(elementId);
    if (errorElement) {
      errorElement.textContent = message;
    }
  }

  // Function to clear all error messages
  function clearErrors() {
    const errorElements = document.querySelectorAll('.error');
    errorElements.forEach((element) => {
      element.textContent = '';
    });
  }

  // Function to validate email format
  function validateEmail(email) {
    // Simple email regex for demonstration purposes
    const re = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
    return re.test(email);
  }
});
13. Debugging and Testing
Scenario: Registration is failing silently. You need to debug.
Objective: Use browser tools to inspect and fix issues.
Task:
• Use Chrome Dev Tools Console and Network tab
• Add breakpoints and inspect variables
• Log form submission steps and check fetch request payload
form.addEventListener('submit', function (event) {
  event.preventDefault();
  
  // Retrieve form values
  const name = form.elements['name'].value.trim();
  const email = form.elements['email'].value.trim();
  const selectedEvent = form.elements['event'].value;

  // Log form values
  console.log('Form Submission:', { name, email, selectedEvent });

  // Proceed with validation and fetch request...
});
14. jQuery and JS Frameworks
Scenario: Use jQuery to simplify DOM tasks.
Objective: Understand and use jQuery.
Task:
• Use $('#registerBtn').click(...) to handle click events
• Use .fadeIn() and .fadeOut() for event cards
• Mention one benefit of moving to frameworks like React or Vue
Task: DOM Manipulation with jQuery
1. Handling Button Click with jQuery
To manage button clicks using jQuery, you can use the following code:

javascript
Copy
Edit
$('#registerBtn').click(function() {
  // Your code here
});
This snippet listens for a click event on the element with the ID registerBtn and executes the provided function when the event occurs.

2. Implementing Fade Effects
To create fade-in and fade-out effects for event cards, you can use:

javascript
Copy
Edit
$('#eventCard').fadeIn();  // Gradually shows the element
$('#eventCard').fadeOut(); // Gradually hides the element
These methods animate the opacity of the selected element, providing a smooth transition.

Transitioning from jQuery to Modern Frameworks
While jQuery simplifies DOM manipulation, modern JavaScript frameworks like React and Vue offer enhanced capabilities for building dynamic user interfaces.

Key Benefits:
Component-Based Architecture: Both React and Vue promote reusable components, making code more modular and maintainable.

Declarative Syntax: These frameworks allow developers to describe the UI state declaratively, leading to more predictable and easier-to-manage code.

Efficient DOM Updates: React and Vue utilize virtual DOMs to efficiently update the actual DOM, improving performance in dynamic applications.

Enhanced State Management: They provide robust mechanisms for managing application state, which is crucial for complex applications.

Considerations:
Learning Curve: Transitioning to frameworks like React or Vue requires learning new concepts and tools, which might have an initial learning curve.

Project Complexity: For simple projects, the overhead of introducing a framework might not be justified. However, for scalable and maintainable applications, frameworks offer significant advantages.


Module 2 - ANSI SQL Using MySQL Exercises
Database Schema
1. User Upcoming Events
List all upcoming events a user is registered for in their city, sorted by date.
SELECT e.title, e.city, e.start_date
FROM Users u
JOIN Registrations r ON u.user_id = r.user_id
JOIN Events e ON r.event_id = e.event_id
WHERE e.status = 'upcoming' AND u.city = e.city
ORDER BY e.start_date;
2. Top Rated Events
Identify events with the highest average rating, considering only those that have received at least 10 feedback submissions.
SELECT e.title, AVG(f.rating) AS avg_rating, COUNT(f.feedback_id) AS feedback_count
FROM Events e
JOIN Feedback f ON e.event_id = f.event_id
GROUP BY e.event_id, e.title
HAVING COUNT(f.feedback_id) >= 10
ORDER BY avg_rating DESC;

3. Inactive Users
Retrieve users who have not registered for any events in the last 90 days.SELECT u.*
FROM Users u
LEFT JOIN Registrations r ON u.user_id = r.user_id AND r.registration_date >= CURDATE() - INTERVAL 90 DAY
WHERE r.registration_id IS NULL;
4. Peak Session Hours
Count how many sessions are scheduled between 10 AM to 12 PM for each event.SELECT e.title, COUNT(s.session_id) AS session_count
FROM Events e
JOIN Sessions s ON e.event_id = s.event_id
WHERE TIME(s.start_time) >= '10:00:00' AND TIME(s.start_time) < '12:00:00'
GROUP BY e.title;
5. Most Active Cities
List the top 5 cities with the highest number of distinct user registrations.SELECT u.city, COUNT(DISTINCT r.user_id) AS user_count
FROM Users u
JOIN Registrations r ON u.user_id = r.user_id
GROUP BY u.city
ORDER BY user_count DESC
LIMIT 5;
6. Event Resource Summary
Generate a report showing the number of resources (PDFs, images, links) uploaded for each event.SELECT e.title,
       SUM(CASE WHEN r.resource_type = 'pdf' THEN 1 ELSE 0 END) AS pdf_count,
       SUM(CASE WHEN r.resource_type = 'image' THEN 1 ELSE 0 END) AS image_count,
       SUM(CASE WHEN r.resource_type = 'link' THEN 1 ELSE 0 END) AS link_count
FROM Events e
LEFT JOIN Resources r ON e.event_id = r.event_id
GROUP BY e.title;
7. Low Feedback Alerts
List all users who gave feedback with a rating less than 3, along with their comments and associated eventSELECT u.full_name, e.title AS event_title, f.rating, f.comments
FROM Feedback f
JOIN Users u ON f.user_id = u.user_id
JOIN Events e ON f.event_id = e.event_id
WHERE f.rating < 3;
8. Sessions per Upcoming Event
Display all upcoming events with the count of sessions scheduled for them.SELECT e.title, COUNT(s.session_id) AS session_count
FROM Events e
LEFT JOIN Sessions s ON e.event_id = s.event_id
WHERE e.status = 'upcoming'
GROUP BY e.title;
9. Organizer Event Summary
For each event organizer, show the number of events created and their current status (upcoming, completed, cancelled).SELECT u.full_name, e.status, COUNT(e.event_id) AS event_count
FROM Users u
JOIN Events e ON u.user_id = e.organizer_id
GROUP BY u.full_name, e.status;
10. Feedback Gap
Identify events that had registrations but received no feedback at all.
SELECT e.title
FROM Events e
JOIN Registrations r ON e.event_id = r.event_id
LEFT JOIN Feedback f ON e.event_id = f.event_id
WHERE f.feedback_id IS NULL
GROUP BY e.title;
11. Daily New User Count
Find the number of users who registered each day in the last 7 days.
SELECT registration_date, COUNT(user_id) AS user_count
FROM Users
WHERE registration_date >= CURDATE() - INTERVAL 7 DAY
GROUP BY registration_date;
12. Event with Maximum Sessions
List the event(s) with the highest number of sessions.
SELECT e.title, COUNT(s.session_id) AS session_count
FROM Events e
JOIN Sessions s ON e.event_id = s.event_id
GROUP BY e.title
ORDER BY session_count DESC
LIMIT 1;
13. Average Rating per City
Calculate the average feedback rating of events conducted in each city.
 e.city, AVG(f.rating) AS avg_rating
FROM Events e
JOIN Feedback f ON e.event_id = f.event_id
GROUP BY e.city;
15. Most Registered Events
List top 3 events based on the total number of user registrations.
Stack Overflow
SELECT e.title, COUNT(r.user_id) AS registration_count
FROM Events e
JOIN Registrations r ON e.event_id = r.event_id
GROUP BY e.title
ORDER BY registration_count DESC
LIMIT 3;
15. Event Session Time Conflict
Identify overlapping sessions within the same event (i.e., session start and end times that conflict).
SELECT s1.session_id AS session1_id, s2.session_id AS session2_id, s1.event_id
FROM Sessions s1
JOIN Sessions s2 ON s1.event_id = s2.event_id AND s1.session_id < s2.session_id
WHERE s1.start_time < s2.end_time AND s2.start_time < s1.end_time;
16. Unregistered Active Users
Find users who created an account in the last 30 days but haven’t registered for any events.
SELECT u.*
FROM Users u
LEFT JOIN Registrations r ON u.user_id = r.user_id
WHERE u.registration_date >= CURDATE() - INTERVAL 30 DAY AND r.registration_id IS NULL;
17. Multi-Session Speakers
Identify speakers who are handling more than one session across all events.
SELECT speaker_name, COUNT(session_id) AS session_count
FROM Sessions
GROUP BY speaker_name
HAVING COUNT(session_id) > 1;
18. Resource Availability Check
List all events that do not have any resources uploaded.
SELECT e.title
FROM Events e
LEFT JOIN Resources r ON e.event_id = r.event_id
WHERE r.resource_id IS NULL;
19. Completed Events with Feedback Summary
For completed events, show total registrations and average feedback rating.
SELECT e.title, COUNT(DISTINCT r.user_id) AS total_registrations, AVG(f.rating) AS avg_rating
FROM Events e
LEFT JOIN Registrations r ON e.event_id = r.event_id
LEFT JOIN Feedback f ON e.event_id = f.event_id
WHERE e.status = 'completed'
GROUP BY e.title;
20. User Engagement Index
For each user, calculate how many events they attended and how many feedbacks they submitted.
SELECT u.full_name,
       COUNT(DISTINCT r.event_id) AS events_attended,
       COUNT(DISTINCT f.feedback_id) AS feedbacks_submitted
FROM Users u
LEFT JOIN Registrations r ON u.user_id = r.user_id
LEFT JOIN Feedback f ON u.user_id = f.user_id
GROUP BY u.full_name;
21. Top Feedback Providers
List top 5 users who have submitted the most feedback entries.
CT u.full_name, COUNT(f.feedback_id) AS feedback_count
FROM Users u
JOIN Feedback f ON u.user_id = f.user_id
GROUP BY u.full_name
ORDER BY feedback_count DESC
LIMIT 5;
23. Duplicate Registrations Check
Detect if a user has been registered more than once for the same event.
SELECT user_id, event_id, COUNT(*) AS registration_count
FROM Registrations
GROUP BY user_id, event_id
HAVING COUNT(*) > 1;
23. Registration Trends
Show a month-wise registration count trend over the past 12 months.
SELECT DATE_FORMAT(registration_date, '%Y-%m') AS month, COUNT(*) AS registration_count
FROM Registrations
WHERE registration_date >= CURDATE() - INTERVAL 12 MONTH
GROUP BY month
ORDER BY month;
24. Average Session Duration per Event
Compute the average duration (in minutes) of sessions in each event.
SELECT e.title, AVG(TIMESTAMPDIFF(MINUTE, s.start_time, s.end_time)) AS avg_duration_minutes
FROM Events e
JOIN Sessions s ON e.event_id = s.event_id
GROUP BY e.title;
25. Events Without Sessions
List all events that currently have no sessions scheduled under them.
SELECT e.title
FROM Events e
LEFT JOIN Sessions s ON e.event_id = s.event_id
WHERE s.session_id IS NULL;
1.Module 3-Core java
**Solution 1:
public class HelloWorld
{
    public static void main(String[] args)
    {
        System.out.println("Hello, World!");
    }
}
**Solution 2:
import java.util.Scanner;
public class Calculator {
    public static void main(String[] args) {
        Scanner s = new Scanner(System.in);
        System.out.println("Enter two numbers:");
        int a = s.nextInt();
        int b = s.nextInt();
        s.nextLine(); 
        System.out.println("Choose an arithmetic operation: Addition, Subtraction, Multiplication, Division");
        String operation = s.nextLine();
        switch (operation) {
            case "Addition":
                System.out.println("Addition of two numbers is: " + (a + b));
                break;
            case "Subtraction":
                System.out.println("Subtraction of two numbers is: " + (a - b));
                break;
            case "Multiplication":
                System.out.println("Multiplication of two numbers is: " + (a * b));
                break;
            case "Division":
                if (b != 0) {
                    System.out.println("Division of two numbers is: " + ((double) a / b));
                } else {
                    System.out.println("Error! Division by zero.");
                }
                break;
            default:
                System.out.println("Invalid operation selected.");
        }
    }
}
**Solution 3:
import java.util.Scanner;
public class EvenOddChecker {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter an integer: ");
        int number = scanner.nextInt();
        if (number % 2 == 0) {
            System.out.println(number + " is even.");
        } else {
            System.out.println(number + " is odd.");
        }
    }
}
**Solution 4:
import java.util.Scanner;
public class LeapYearChecker {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);\
        System.out.print("Enter a year: ");
        int year = scanner.nextInt();
        if (year % 4 == 0) {
            if (year % 100 == 0) {
                if (year % 400 == 0) {
                    System.out.println(year + " is a leap year.");
                } 
                else 
                {
                    System.out.println(year + " is not a leap year.");
                }
            } 
            else 
            {
                System.out.println(year + " is a leap year.");
            }
        } 
        else
        {
            System.out.println(year + " is not a leap year.");
        }
    }
}
**Solution 5:
import java.util.Scanner;
public class MultiplicationTable {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter a number: ");
        int number = scanner.nextInt();
        for (int i = 1; i <= 10; i++) {
            int result = number * i;
            System.out.println(number + " x " + i + " = " + result);
        }
    }
}
**Solution 6:
public class DataTypeDemo {
    public static void main(String[] args) {
        int myInt = 25;
        float myFloat = 3.14f;
        double myDouble = 123.456;
        char myChar = 'A';
        boolean myBoolean = true;
        System.out.println("Integer value: " + myInt);
        System.out.println("Float value: " + myFloat);
        System.out.println("Double value: " + myDouble);
        System.out.println("Character value: " + myChar);
        System.out.println("Boolean value: " + myBoolean);
    }
}
**Solution 7:
public class TypeCastingExample {
    public static void main(String[] args) {
        double myDouble = 9.78;
        int myInt = (int) myDouble;
        System.out.println("Original double value: " + myDouble);
        System.out.println("After casting to int: " + myInt);
        int anotherInt = 42;
        double anotherDouble = anotherInt;
        System.out.println("Original int value: " + anotherInt);
        System.out.println("After casting to double: " + anotherDouble);
    }
}
**Solution 8:
public class OperatorPrecedenceDemo {
    public static void main(String[] args) {
        int result1 = 10 + 5 * 2;
        int result2 = (10 + 5) * 2;
        int result3 = 100 / 10 + 5;
        int result4 = 100 / (10 + 5);
        int result5 = 2 + 3 * 4 - 5;
        int result6 = 2 + (3 * (4 - 5));
        System.out.println("Result 1 (10 + 5 * 2): " + result1);
        System.out.println("Result 2 ((10 + 5) * 2): " + result2);
        System.out.println("Result 3 (100 / 10 + 5): " + result3);
        System.out.println("Result 4 (100 / (10 + 5)): " + result4);
        System.out.println("Result 5 (2 + 3 * 4 - 5): " + result5);
        System.out.println("Result 6 (2 + (3 * (4 - 5))): " + result6);
    }
}
**Solution 9:
import java.util.Scanner;
public class GradeCalculator {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter marks out of 100: ");
        int marks = scanner.nextInt();
        if (marks < 0 || marks > 100) {
            System.out.println("Invalid input. Please enter marks between 0 and 100.");
        } else {
            char grade;
            if (marks >= 90) {
                grade = 'A';
            } else if (marks >= 80) {
                grade = 'B';
            } else if (marks >= 70) {
                grade = 'C';
            } else if (marks >= 60) {
                grade = 'D';
            } else {
                grade = 'F';
            }
            System.out.println("Grade: " + grade);
        }
    }
}
**Solution 10:
import java.util.Scanner;
public class NumberGuessingGame {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int targetNumber = 1 + (int) (100 * Math.random());
        int userGuess = 0;
        int attempts = 0;
        System.out.println("Welcome to the Number Guessing Game!");
        System.out.println("I have selected a number between 1 and 100.");
        System.out.println("Try to guess it!");
        while (userGuess != targetNumber) {
            System.out.print("Enter your guess: ");
            userGuess = scanner.nextInt();
            attempts++;
            if (userGuess < targetNumber) {
                System.out.println("The number is higher than " + userGuess + ". Try again.");
            } else if (userGuess > targetNumber) {
                System.out.println("The number is lower than " + userGuess + ". Try again.");
            } else {
                System.out.println("Congratulations! You guessed the correct number in " + attempts + " attempts.");
            }
        }
    }
}
**Solution 11:
import java.util.Scanner;
public class FactorialCalculator {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter a non-negative integer: ");
        int number = scanner.nextInt();
        if (number < 0) {
            System.out.println("Factorial is not defined for negative numbers.");
        } else {
            long factorial = 1;
            for (int i = 1; i <= number; i++) {
                factorial *= i;
            }
            System.out.println("Factorial of " + number + " is: " + factorial);
        }
    }
}
**Solution 12:
public class Calculator {
    public int add(int a, int b) {
        return a + b;
    }
    public double add(double a, double b) {
        return a + b;
    }
    public int add(int a, int b, int c) {
        return a + b + c;
    }

    public static void main(String[] args) {
        Calculator calc = new Calculator();
        System.out.println("Sum of a and b (int): " + calc.add(5, 10));
        System.out.println("Sum of a and b (double): " + calc.add(5.5, 10.5));
        System.out.println("Sum of a, b, and c (int): " + calc.add(5, 10, 15));
    }
}
**Solution 13:
import java.util.Scanner;
public class Fibonacci {
    // Recursive method to calculate the nth Fibonacci number
    public static int fibonacci(int n) {
        if (n <= 1) {
            return n;
        }
        return fibonacci(n - 1) + fibonacci(n - 2);
    }
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter a positive integer n: ");
        int n = scanner.nextInt();
        if (n < 0) {
            System.out.println("Please enter a positive integer.");
        } else {
            System.out.println("The " + n + "th Fibonacci number is: " + fibonacci(n));
        }
    }
}
**Solution 14:
import java.util.Scanner;
public class ArraySumAverage {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter the number of elements: ");
        int n = scanner.nextInt();
        int[] numbers = new int[n];
        System.out.println("Enter the elements:");
        int sum = 0;
        for (int i = 0; i < n; i++) {
            numbers[i] = scanner.nextInt();
            sum += numbers[i]; 
        }
        double average = (double) sum / n;
        System.out.println("Sum: " + sum);
        System.out.println("Average: " + average);
    }
}
**Solution 15:
import java.util.Scanner;
public class StringReversal {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter a string: ");
        String input = scanner.nextLine();
        StringBuilder reversed = new StringBuilder();
        for (int i = input.length() - 1; i >= 0; i--) {
            reversed.append(input.charAt(i));
        }
        System.out.println("Reversed string: " + reversed.toString());
    }
}
**Solution 16:
import java.util.Scanner;
public class PalindromeChecker {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter a string: ");
        String input = scanner.nextLine();
        String cleanedInput = input.replaceAll("[^a-zA-Z0-9]", "").toLowerCase();
        if (isPalindrome(cleanedInput)) {
            System.out.println("\"" + input + "\" is a palindrome.");
        } else {
            System.out.println("\"" + input + "\" is not a palindrome.");
        }
    }
    private static boolean isPalindrome(String str) {
        int left = 0;
        int right = str.length() - 1;
        while (left < right) {
            if (str.charAt(left) != str.charAt(right)) {
                return false;
            }
            left++;
            right--;
        }
        return true;
    }
}
**Solution 17:
class Car {
    String make;
    String model;
    int year;
    public Car(String make, String model, int year) {
        this.make = make;
        this.model = model;
        this.year = year;
    }
    public void displayDetails() {
        System.out.println("Car Details:");
        System.out.println("Make: " + make);
        System.out.println("Model: " + model);
        System.out.println("Year: " + year);
    }
}
public class Main {
    public static void main(String[] args) {
        Car car1 = new Car("Toyota", "Corolla", 2020);
        Car car2 = new Car("Honda", "Civic", 2022);
        car1.displayDetails();
        car2.displayDetails();
    }
}
**Solution 18:
    public void makeSound() {
        System.out.println("The animal makes a sound.");
    }
}
class Dog extends Animal {
    public void makeSound() {
        System.out.println("Bark");
    }
}

public class Main {
    public static void main(String[] args) {
        Animal animal = new Animal();
        animal.makeSound(); 
        Dog dog = new Dog();
        dog.makeSound(); 
        Animal myDog = new Dog();
        myDog.makeSound(); 
    }
}
**Solution 19:
interface Playable {
    void play();
}
class Guitar implements Playable {
    public void play() {
        System.out.println("Strumming the guitar: 'Strum strum strum!'");
    }
}
class Piano implements Playable {
    public void play() {
        System.out.println("Playing the piano: 'Ding dong ding!'");
    }
}
public class Main {
    public static void main(String[] args) {
        Playable guitar = new Guitar();
        Playable piano = new Piano();
        guitar.play();
        piano.play();
    }
}
**Solution 20:
import java.util.Scanner;
public class DivisionByZeroExample {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter the numerator: ");
        int numerator = scanner.nextInt();
        System.out.print("Enter the denominator: ");
        int denominator = scanner.nextInt();
        try {
            int result = numerator / denominator;
            System.out.println("Result: " + result);
        } catch (ArithmeticException e) {
            System.out.println("Error: Cannot divide by zero.");
        } finally {
            scanner.close();
        }
    }
}
**Solution 21:
import java.util.Scanner;
class InvalidAgeException extends Exception {
    public InvalidAgeException(String message) {
        super(message);
    }
}

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter your age: ");
        int age = scanner.nextInt();

        try {
            // Step 2: Validate the age
            if (age < 18) {
                throw new InvalidAgeException("Age must be 18 or above.");
            } else {
                System.out.println("Age is valid.");
            }
        } catch (InvalidAgeException e) {
            System.out.println("Caught Exception: " + e.getMessage());
        } finally {
            scanner.close();
        }
    }
}
**Solution 22:
import java.io.FileWriter;
import java.io.IOException;
import java.io.PrintWriter;
import java.util.Scanner;
public class FileWritingExample {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter a string: ");
        String userInput = scanner.nextLine();
        try (PrintWriter writer = new PrintWriter(new FileWriter("output.txt"))) {
            writer.println(userInput);
            System.out.println("Data has been written to output.txt.");
        } catch (IOException e) {
            System.out.println("An error occurred while writing to the file.");
            e.printStackTrace();
        } finally {
            scanner.close();
        }
    }
}
**Solution 23:
import java.io.BufferedReader;
import java.io.FileReader;
import java.io.IOException;
public class FileReadingExample {
    public static void main(String[] args) {
        String filePath = "output.txt"; // Specify the path to your file
        try (BufferedReader reader = new BufferedReader(new FileReader(filePath))) {
            String line;
            while ((line = reader.readLine()) != null) {
                System.out.println(line); // Display each line
            }
        } catch (IOException e) {
            System.err.println("An error occurred while reading the file: " + e.getMessage());
        }
    }
}
**Solution 24:
import java.util.ArrayList;
import java.util.Scanner;
public class StudentNames {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        ArrayList<String> students = new ArrayList<>();
        System.out.println("Enter student names. Type 'done' to finish.");
        while (true) {
            System.out.print("Enter a name: ");
            String name = scanner.nextLine();
            if (name.equalsIgnoreCase("done")) {
                break;
            }

            students.add(name);
        }

        System.out.println("\nList of student names entered:");
        for (String student : students) {
            System.out.println(student);
        }
    }
}
**SOlution 25:
import java.util.HashMap;
import java.util.Scanner;
public class StudentIDNameMap {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        HashMap<Integer, String> studentMap = new HashMap<>();
        while (true) {
            System.out.println("\nMenu:");
            System.out.println("1. Add Student");
            System.out.println("2. Retrieve Student Name by ID");
            System.out.println("3. Display All Students");
            System.out.println("4. Exit");
            System.out.print("Choose an option: ");
            int choice = scanner.nextInt();
            scanner.nextLine();  // Consume newline
            switch (choice) {
                case 1:
                    System.out.print("Enter Student ID: ");
                    int id = scanner.nextInt();
                    scanner.nextLine();  // Consume newline
                    System.out.print("Enter Student Name: ");
                    String name = scanner.nextLine();
                    studentMap.put(id, name);
                    System.out.println("Student added successfully.");
                    break;
                case 2:
                    System.out.print("Enter Student ID to retrieve name: ");
                    int searchId = scanner.nextInt();
                    String studentName = studentMap.get(searchId);
                    if (studentName != null) {
                        System.out.println("Student Name: " + studentName);
                    } else {
                        System.out.println("No student found with ID: " + searchId);
                    }
                    break;

                case 3:
                    if (studentMap.isEmpty()) {
                        System.out.println("No students in the system.");
                    } else {
                        System.out.println("All Students:");
                        for (Integer studentId : studentMap.keySet()) {
                            System.out.println("ID: " + studentId + ", Name: " + studentMap.get(studentId));
                        }
                    }
                    break;

                case 4:
                    System.out.println("Exiting the program.");
                    scanner.close();
                    return;

                default:
                    System.out.println("Invalid choice. Please try again.");
            }
        }
    }
}
**Solution 26:
public class ThreadExample {
    public static void main(String[] args) {
        Thread thread1 = new Thread(new Runnable() {
            @Override
            public void run() {
                for (int i = 0; i < 5; i++) {
                    System.out.println("Thread 1: Message " + (i + 1));
                    try {
                        Thread.sleep(500); // Sleep for 500 milliseconds
                    } catch (InterruptedException e) {
                        System.out.println(e);
                    }
                }
            }
        });

        Thread thread2 = new Thread(new Runnable() {
            @Override
            public void run() {
                for (int i = 0; i < 5; i++) {
                    System.out.println("Thread 2: Message " + (i + 1));
                    try {
                        Thread.sleep(500); // Sleep for 500 milliseconds
                    } catch (InterruptedException e) {
                        System.out.println(e);
                    }
                }
            }
        });

        // Start both threads
        thread1.start();
        thread2.start();
    }
}
**Solution 27:
import java.util.Arrays;
import java.util.List;
public class LambdaSortExample {
    public static void main(String[] args) {
        List<String> fruits = Arrays.asList("Banana", "Apple", "Mango", "Pineapple", "Grapes");
        System.out.println("Original List:");
        fruits.forEach(fruit -> System.out.println(fruit));
        fruits.sort((fruit1, fruit2) -> fruit1.compareTo(fruit2));
        System.out.println("\nSorted List:");
        fruits.forEach(fruit -> System.out.println(fruit));
    }
}
**Solution 28:
import java.util.Arrays;
import java.util.List;
import java.util.stream.Collectors;
public class EvenNumberFilter {
    public static void main(String[] args) {
        List<Integer> numbers = Arrays.asList(1, 2, 3, 4, 5, 6, 7, 8, 9, 10);
        List<Integer> evenNumbers = numbers.stream()
                                           .filter(n -> n % 2 == 0)
                                           .collect(Collectors.toList());
        System.out.println("Even numbers: " + evenNumbers);
    }
}
**Solution 29:
import java.util.Arrays;
import java.util.List;
import java.util.stream.Collectors;
public class PersonExample {
    public record Person(String name, int age) {}
    public static void main(String[] args) {
        Person alice = new Person("Alice", 30);
        Person bob = new Person("Bob", 25);
        Person charlie = new Person("Charlie", 35);
        List<Person> people = Arrays.asList(alice, bob, charlie);
        System.out.println("All Persons:");
        people.forEach(person -> System.out.println(person));
        List<Person> filteredPeople = people.stream()
                                             .filter(p -> p.age() >= 30)
                                             .collect(Collectors.toList());
        System.out.println("\nPersons aged 30 and above:");
        filteredPeople.forEach(person -> System.out.println(person));
    }
}
**Soloution 30:
public class TypeChecker {
    public static void main(String[] args) {
        System.out.println(checkType("Hello"));
        System.out.println(checkType(42));
        System.out.println(checkType(3.14));
        System.out.println(checkType(true));
        System.out.println(checkType(null));
    }
    public static String checkType(Object obj) {
        return switch (obj) {
            case String s -> "It's a String: " + s;
            case Integer i -> "It's an Integer: " + i;
            case Double d -> "It's a Double: " + d;
            case Boolean b -> "It's a Boolean: " + b;
            case null -> "It's null";
            default -> "Unknown type: " + obj.getClass().getName();
        };
    }
}
**Solution 31:
CREATE DATABASE school;
USE school;

CREATE TABLE students (
    id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(100),
    age INT
);

INSERT INTO students (name, age) VALUES
('Alice', 20),
('Bob', 22),
('Charlie', 23);
import java.sql.*;

public class JdbcExample {
    public static void main(String[] args) {
        String url = "jdbc:mysql:
        String user = "root";
        String password = "your_password";
        String query = "SELECT id, name, age FROM students";

        try (
            Connection conn = DriverManager.getConnection(url, user, password);
            Statement stmt = conn.createStatement();
            // Execute query and get result set
            ResultSet rs = stmt.executeQuery(query)
        ) {
            while (rs.next()) {
                int id = rs.getInt("id");
                String name = rs.getString("name");
                int age = rs.getInt("age");
                System.out.println("ID: " + id + ", Name: " + name + ", Age: " + age);
            }
        } catch (SQLException e) {
            e.printStackTrace();
        }
    }
}
**Solution 32:
CREATE DATABASE school;
USE school;

CREATE TABLE students (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    age INT
);

-- Sample data
INSERT INTO students (name, age) VALUES
('Alice', 20),
('Bob', 22),
('Charlie', 23);
import java.sql.*;
public class StudentDAO {
    private static final String URL = "jdbc:mysql://localhost:3306/school";
    private static final String USER = "root";
    private static final String PASSWORD = "your_password"; // Replace with your MySQL password

    // Method to insert a new student
    public void insertStudent(String name, int age) {
        String query = "INSERT INTO students (name, age) VALUES (?, ?)";
        try (Connection conn = DriverManager.getConnection(URL, USER, PASSWORD);
             PreparedStatement stmt = conn.prepareStatement(query)) {
            stmt.setString(1, name);
            stmt.setInt(2, age);
            int rowsAffected = stmt.executeUpdate();
            System.out.println("Inserted " + rowsAffected + " row(s).");
        } catch (SQLException e) {
            e.printStackTrace();
        }
    }

    // Method to update an existing student's details
    public void updateStudent(int id, String name, int age) {
        String query = "UPDATE students SET name = ?, age = ? WHERE id = ?";
        try (Connection conn = DriverManager.getConnection(URL, USER, PASSWORD);
             PreparedStatement stmt = conn.prepareStatement(query)) {
            stmt.setString(1, name);
            stmt.setInt(2, age);
            stmt.setInt(3, id);
            int rowsAffected = stmt.executeUpdate();
            if (rowsAffected > 0) {
                System.out.println("Updated student with ID " + id);
            } else {
                System.out.println("No student found with ID " + id);
            }
        } catch (SQLException e) {
            e.printStackTrace();
        }
    }

    // Method to display all students
    public void displayStudents() {
        String query = "SELECT id, name, age FROM students";
        try (Connection conn = DriverManager.getConnection(URL, USER, PASSWORD);
             Statement stmt = conn.createStatement();
             ResultSet rs = stmt.executeQuery(query)) {
            while (rs.next()) {
                int id = rs.getInt("id");
                String name = rs.getString("name");
                int age = rs.getInt("age");
                System.out.println("ID: " + id + ", Name: " + name + ", Age: " + age);
            }
        } catch (SQLException e) {
            e.printStackTrace();
        }
    }
}
**Solution 33:
CREATE DATABASE school;
USE school;

CREATE TABLE students (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    age INT
);

-- Sample data
INSERT INTO students (name, age) VALUES
('Alice', 20),
('Bob', 22),
('Charlie', 23);
import java.sql.*;

public class StudentDAO {
    private static final String URL = "jdbc:mysql://localhost:3306/school";
    private static final String USER = "root";
    private static final String PASSWORD = "your_password"; // Replace with your MySQL password

    // Method to insert a new student
    public void insertStudent(String name, int age) {
        String query = "INSERT INTO students (name, age) VALUES (?, ?)";
        try (Connection conn = DriverManager.getConnection(URL, USER, PASSWORD);
             PreparedStatement stmt = conn.prepareStatement(query)) {
            stmt.setString(1, name);
            stmt.setInt(2, age);
            int rowsAffected = stmt.executeUpdate();
            System.out.println("Inserted " + rowsAffected + " row(s).");
        } catch (SQLException e) {
            e.printStackTrace();
        }
    }

    // Method to update an existing student's details
    public void updateStudent(int id, String name, int age) {
        String query = "UPDATE students SET name = ?, age = ? WHERE id = ?";
        try (Connection conn = DriverManager.getConnection(URL, USER, PASSWORD);
             PreparedStatement stmt = conn.prepareStatement(query)) {
            stmt.setString(1, name);
            stmt.setInt(2, age);
            stmt.setInt(3, id);
            int rowsAffected = stmt.executeUpdate();
            if (rowsAffected > 0) {
                System.out.println("Updated student with ID " + id);
            } else {
                System.out.println("No student found with ID " + id);
            }
        } catch (SQLException e) {
            e.printStackTrace();
        }
    }

    // Method to display all students
    public void displayStudents() {
        String query = "SELECT id, name, age FROM students";
        try (Connection conn = DriverManager.getConnection(URL, USER, PASSWORD);
             Statement stmt = conn.createStatement();
             ResultSet rs = stmt.executeQuery(query)) {
            while (rs.next()) {
                int id = rs.getInt("id");
                String name = rs.getString("name");
                int age = rs.getInt("age");
                System.out.println("ID: " + id + ", Name: " + name + ", Age: " + age);
            }
        } catch (SQLException e) {
            e.printStackTrace();
        }
    }
}
public class Main {
    public static void main(String[] args) {
        StudentDAO dao = new StudentDAO();

        // Insert a new student
        dao.insertStudent("David", 24);

        // Update an existing student's details
        dao.updateStudent(1, "Alice Johnson", 21);

        // Display all students
        dao.displayStudents();
    }
}
**Solution 34:
project-root/
├── src/
│   ├── com.utils/
│   │   ├── module-info.java
│   │   └── com/utils/Utils.java
│   └── com.greetings/
│       ├── module-info.java
│       └── com/greetings/Greeting.java
└── out/
module com.utils {
    exports com.utils;
}
package com.utils;

public class Utils {
    public static String getGreeting() {
        return "Hello from Utils!";
    }
}
module com.greetings {
    requires com.utils;
}
package com.greetings;

import com.utils.Utils;

public class Greeting {
    public static void main(String[] args) {
        System.out.println(Utils.getGreeting());
    }
}
javac -d out/com.utils src/com.utils/module-info.java src/com/utils/Utils.java
javac -d out/com.greetings --module-path out -d out/com.greetings src/com.greetings/module-info.java src/com/greetings/Greeting.java
java --module-path out -m com.greetings/com.greetings.Greeting
**Solution 35:
import java.io.*;
import java.net.*;
import java.util.*;

public class ChatServer {
    private static final int PORT = 12345;
    private static Set<PrintWriter> clientWriters = new HashSet<>();

    public static void main(String[] args) throws IOException {
        System.out.println("Chat server started...");
        try (ServerSocket serverSocket = new ServerSocket(PORT)) {
            while (true) {
                new ClientHandler(serverSocket.accept()).start();
            }
        }
    }

    private static class ClientHandler extends Thread {
        private Socket socket;
        private PrintWriter out;
        private BufferedReader in;

        public ClientHandler(Socket socket) {
            this.socket = socket;
        }

        public void run() {
            try {
                in = new BufferedReader(new InputStreamReader(socket.getInputStream()));
                out = new PrintWriter(socket.getOutputStream(), true);
                synchronized (clientWriters) {
                    clientWriters.add(out);
                }
                String message;
                while ((message = in.readLine()) != null) {
                    System.out.println("Received: " + message);
                    synchronized (clientWriters) {
                        for (PrintWriter writer : clientWriters) {
                            writer.println(message);
                        }
                    }
                }
            } catch (IOException e) {
                System.out.println("Error handling client: " + e.getMessage());
            } finally {
                try {
                    socket.close();
                } catch (IOException e) {
                    System.out.println("Error closing socket: " + e.getMessage());
                }
                synchronized (clientWriters) {
                    clientWriters.remove(out);
                }
            }
        }
    }
}
import java.io.*;
import java.net.*;

public class ChatClient {
    private static final String SERVER_ADDRESS = "localhost";
    private static final int SERVER_PORT = 12345;

    public static void main(String[] args) throws IOException {
        try (Socket socket = new Socket(SERVER_ADDRESS, SERVER_PORT);
             BufferedReader in = new BufferedReader(new InputStreamReader(socket.getInputStream()));
             PrintWriter out = new PrintWriter(socket.getOutputStream(), true);
             BufferedReader userInput = new BufferedReader(new InputStreamReader(System.in))) {

            System.out.println("Connected to the chat server.");
            new ReadThread(in).start();

            String message;
            while ((message = userInput.readLine()) != null) {
                out.println(message);
            }
        }
    }

    private static class ReadThread extends Thread {
        private BufferedReader in;

        public ReadThread(BufferedReader in) {
            this.in = in;
        }

        public void run() {
            String message;
            try {
                while ((message = in.readLine()) != null) {
                    System.out.println(message);
                }
            } catch (IOException e) {
                System.out.println("Error reading from server: " + e.getMessage());
            }
        }
    }
}
**Solution 36:
<dependencies>
    <!-- Jackson for JSON parsing -->
    <dependency>
        <groupId>com.fasterxml.jackson.core</groupId>
        <artifactId>jackson-databind</artifactId>
        <version>2.13.1</version>
    </dependency>
    <!-- Gson for JSON parsing -->
    <dependency>
        <groupId>com.google.code.gson</groupId>
        <artifactId>gson</artifactId>
        <version>2.8.8</version>
    </dependency>
</dependencies>
import java.net.URI;
import java.net.http.HttpClient;
import java.net.http.HttpRequest;
import java.net.http.HttpResponse;
import java.io.IOException;

public class GitHubApiClient {
    public static void main(String[] args) throws IOException, InterruptedException {
        String user = "octocat"; // Replace with any GitHub username
        String url = "https://api.github.com/users/" + user;

        HttpClient client = HttpClient.newHttpClient();
        HttpRequest request = HttpRequest.newBuilder()
                .uri(URI.create(url))
                .header("Accept", "application/vnd.github.v3+json")
                .build();

        HttpResponse<String> response = client.send(request, HttpResponse.BodyHandlers.ofString());

        System.out.println("Status Code: " + response.statusCode());
        System.out.println("Response Body: " + response.body());
    }
}
import com.fasterxml.jackson.databind.JsonNode;
import com.fasterxml.jackson.databind.ObjectMapper;

public class JacksonParser {
    public static void main(String[] args) throws IOException {
        String jsonResponse = "{ \"login\": \"octocat\", \"id\": 1 }"; // Replace with actual response

        ObjectMapper mapper = new ObjectMapper();
        JsonNode rootNode = mapper.readTree(jsonResponse);

        String login = rootNode.path("login").asText();
        int id = rootNode.path("id").asInt();

        System.out.println("Login: " + login);
        System.out.println("ID: " + id);
    }
}
import com.google.gson.JsonObject;
import com.google.gson.JsonParser;

public class GsonParser {
    public static void main(String[] args) {
        String jsonResponse = "{ \"login\": \"octocat\", \"id\": 1 }"; // Replace with actual response

        JsonObject jsonObject = JsonParser.parseString(jsonResponse).getAsJsonObject();

        String login = jsonObject.get("login").getAsString();
        int id = jsonObject.get("id").getAsInt();

        System.out.println("Login: " + login);
        System.out.println("ID: " + id);
    }
}
HttpRequest request = HttpRequest.newBuilder()
        .uri(URI.create(url))
        .header("Accept", "application/vnd.github.v3+json")
        .header("Authorization", "Bearer YOUR_PERSONAL_ACCESS_TOKEN")
        .build();
**Solution 37:
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
javac HelloWorld.java
javap -c HelloWorld
Compiled from "HelloWorld.java"
public class HelloWorld {
  public HelloWorld();
    Code:
       0: aload_0
       1: invokespecial #1    // Method java/lang/Object."<init>":()V
       4: return
  public static void main(java.lang.String[]);
    Code:
       0: getstatic     #2    // Field java/lang/System.out:Ljava/io/PrintStream;
       3: ldc           #3    // String Hello, World!
       5: invokevirtual #4    // Method java/io/PrintStream.println:(Ljava/lang/String;)V
       8: return
}
**Solution 38:
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
javac HelloWorld.java
java -jar cfr-0.152.jar HelloWorld.class --outputdir ./decompiled

**Solution 39:
public class Sample {
    public void greet(String name) {
        System.out.println("Hello, " + name + "!");
    }

    private void secret() {
        System.out.println("This is a secret method.");
    }
}
import java.lang.reflect.Method;

public class ReflectionExample {
    public static void main(String[] args) {
        try {
            // Load the Sample class
            Class<?> clazz = Class.forName("Sample");

            // List all declared methods
            Method[] methods = clazz.getDeclaredMethods();
            for (Method method : methods) {
                System.out.println("Method: " + method.getName());
            }
        } catch (ClassNotFoundException e) {
            e.printStackTrace();
        }
    }
}
import java.lang.reflect.Method;

public class ReflectionExample {
    public static void main(String[] args) {
        try {
            // Load the Sample class
            Class<?> clazz = Class.forName("Sample");

            // Create an instance of Sample
            Object sampleInstance = clazz.getDeclaredConstructor().newInstance();

            // Invoke the public greet method
            Method greetMethod = clazz.getDeclaredMethod("greet", String.class);
            greetMethod.invoke(sampleInstance, "Alice");

            // Invoke the private secret method
            Method secretMethod = clazz.getDeclaredMethod("secret");
            secretMethod.setAccessible(true); // Allow access to private method
            secretMethod.invoke(sampleInstance);
        } catch (Exception e) {
            e.printStackTrace();
        }
    }
}
**Solution 40:
public class VirtualThreadExample {
    public static void main(String[] args) {
        for (int i = 0; i < 100_000; i++) {
            Thread.startVirtualThread(() -> {
                // Simulate task
                try {
                    Thread.sleep(100);
                } catch (InterruptedException e) {
                    Thread.currentThread().interrupt();
                }
            });
        }
    }
}
**Solution 41:
import java.util.concurrent.Callable;

public class MyTask implements Callable<String> {
    @Override
    public String call() throws Exception {
        // Simulate a task by sleeping for 2 seconds
        Thread.sleep(2000);
        return "Task Completed";
    }
}
import java.util.concurrent.*;

public class ExecutorServiceExample {
    public static void main(String[] args) {
        // Create a fixed thread pool with 5 threads
        ExecutorService executor = Executors.newFixedThreadPool(5);

        // Submit 10 tasks
        List<Future<String>> results = new ArrayList<>();
        for (int i = 0; i < 10; i++) {
            results.add(executor.submit(new MyTask()));
        }

        // Retrieve and print the results
        for (Future<String> future : results) {
            try {
                // This will block until the result is available
                System.out.println(future.get());
            } catch (InterruptedException | ExecutionException e) {
                e.printStackTrace();
            }
        }

        // Shut down the executor
        executor.shutdown();
    }
}

























