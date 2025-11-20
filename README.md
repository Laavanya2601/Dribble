# Project Responsive Web Design using Bootstrap
## Date:

## AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.


## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project. 

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

### Step 5:
Create a HTML file and include the needed Bootstrap components.

### Step 6:
Publish the website in the LocalHost.

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>South Indian Actors Gallery</title>

  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: #f5f5f5;
    }

    .navbar {
      display: flex;
      justify-content: space-between;
      align-items: center;
      background: #2d2d2d;
      color: white;
      padding: 10px 20px;
    }

    .navbar .logo {
      font-size: 1.5rem;
      font-weight: bold;
    }

    .navbar .nav-links,
    .navbar .auth {
      display: flex;
      gap: 15px;
    }

    .navbar a {
      color: white;
      text-decoration: none;
    }

    .sub-header {
      background: #fafafa;
      padding: 20px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
    }

    .sub-actions button {
      margin-left: 10px;
      padding: 8px 12px;
      border: 1px solid #ccc;
      background: white;
      cursor: pointer;
    }

    .sign-up {
      background: #ea4c89;
      color: white;
      border: none;
    }

    .filter-bar {
      display: flex;
      gap: 10px;
      padding: 15px 20px;
      background: white;
      border-bottom: 1px solid #ddd;
    }

    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
      gap: 20px;
      padding: 20px;
    }

    .card {
      background: white;
      border-radius: 6px;
      overflow: hidden;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
      transition: transform 0.2s;
    }

    .card:hover {
      transform: translateY(-4px);
    }

    .card img {
      width: 100%;
      height: 250px;
      object-fit: cover;
      object-position: center;
      display: block;
    }

    .card .info {
      padding: 10px;
    }

    .card .author {
      font-weight: bold;
      margin: 0 0 4px;
    }

    .card .stats {
      font-size: 0.8rem;
      color: #666;
      margin: 0;
    }
  </style>
</head>
<body>

  <header class="navbar">
    <div class="logo">Dribbble</div>
    <nav>
      <ul class="nav-links">
        <li><a href="#">Shots</a></li>
        <li><a href="#">Designers</a></li>
        <li><a href="#">Teams</a></li>
        <li><a href="#">Community</a></li>
        <li><a href="#">Jobs</a></li>
      </ul>
    </nav>
    <div class="auth">
      <a href="#">Sign up</a>
      <a href="#">Sign in</a>
    </div>
  </header>

  <section class="sub-header">
    <p>Top South Indian Actors — Real Photos</p>
    <div class="sub-actions">
      <button>Learn more</button>
      <button class="sign-up">Sign up</button>
    </div>
  </section>

  <section class="filter-bar">
    <select><option>Popular</option></select>
    <select><option>Actors</option></select>
    <select><option>Now</option></select>
  </section>

  <main class="grid">

    <div class="card">
      <img src="i1.jpg" alt="Vijay">
      <div class="info">
        <p class="author">Thalapathy Vijay</p>
        <p class="stats">110M views • 14M comments • 100M likes</p>
      </div>
    </div>

    <div class="card">
      <img src="i10.jpg" alt="Allu Arjun">
      <div class="info">
        <p class="author">Allu Arjun</p>
        <p class="stats">2,222 views • 13 comments • 236 likes</p>
      </div>
    </div>

    <div class="card">
      <img src="i11.jpg" alt="Vijay Deverakonda">
      <div class="info">
        <p class="author">Vijay Deverakonda</p>
        <p class="stats">3,985 views • 17 comments • 264 likes</p>
      </div>
    </div>

    <div class="card">
      <img src="i9.jpg" alt="Rajinikanth">
      <div class="info">
        <p class="author">Rajinikanth</p>
        <p class="stats">2.9M views • 232k comments • 953k likes</p>
      </div>
    </div>

    <div class="card">
      <img src="i8.jpg" alt="Mahesh Babu">
      <div class="info">
        <p class="author">Mahesh Babu</p>
        <p class="stats">2,602 views • 23 comments • 186 likes</p>
      </div>
    </div>

    <div class="card">
      <img src="i7.jpg" alt="Suriya">
      <div class="info">
        <p class="author">Suriya</p>
        <p class="stats">2,602 views • 23 comments • 186 likes</p>
      </div>
    </div>

    <div class="card">
      <img src="i6.jpg" alt="Yash">
      <div class="info">
        <p class="author">Yash</p>
        <p class="stats">2,602 views • 23 comments • 186 likes</p>
      </div>
    </div>

    <div class="card">
      <img src="i5.jpg" alt="Jr NTR">
      <div class="info">
        <p class="author">Jr NTR</p>
        <p class="stats">2,602 views • 23 comments • 186 likes</p>
      </div>
    </div>

    <div class="card">
      <img src="i4.jpg" alt="Ram Charan">
      <div class="info">
        <p class="author">Ram Charan</p>
        <p class="stats">2,602 views • 23 comments • 186 likes</p>
      </div>
    </div>

    <div class="card">
      <img src="i3.jpg" alt="Dhanush">
      <div class="info">
        <p class="author">Dhanush</p>
        <p class="stats">2,602 views • 23 comments • 186 likes</p>
      </div>
    </div>

    <div class="card">
      <img src="i2.jpg" alt="Prabhas">
      <div class="info">
        <p class="author">Prabhas</p>
        <p class="stats">2,602 views • 23 comments • 186 likes</p>
      </div>
    </div>

    <div class="card">
      <img src="i0.jpg" alt="Karthi">
      <div class="info">
        <p class="author">Karthi</p>
        <p class="stats">2,602 views • 23 comments • 186 likes</p>
      </div>
    </div>

  </main>

</body>
</html>
```


## OUTPUT:
<img width="1918" height="1079" alt="image" src="https://github.com/user-attachments/assets/4c6407c3-27f9-4d52-9a95-34d8f429fc1a" />


## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
