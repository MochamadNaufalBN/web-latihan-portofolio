<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" href="style.css" />
    <title>Mochamad Naufal Bayu Nugraha</title>
</head>
<body>
    <div class="container">
        <div class="sidebar">
            <nav>
                <ul>
                    <li><a href="">About</a></li>
                    <li><a href="">Portfolio</a></li>
                    <li><a href="">Blog</a></li>
                    <li><a href="">Contact</a></li>
                </ul>
            </nav>
        </div>
        <main class="content">
            <section class="hero">
                <img src="online.png" alt="Profile Image" />
                <div class="hero-content">
                    <h1>Profesi</h1>
                    <h2>Junior Content Writer at Dicoding</h2>
                    <p>
                       halo namaku naufal sedang dalam pembelajaran kode html mohon bantuannya.
                      sedikit sedikit lama lama akan jadi bukit.
                    </p>
                    <a href="" class="action-btn">Profile Saya</a>
                </div>
            </section>
        </main>
        <div class="footer">
            <footer>
                <ul>
                    <li>
                        <img src="instagram.png" alt="Instagram Logo" />
                        <a href="#"><p>Instagram</p></a>
                    </li>
                    <li>
                        <img src="facebook.png" alt="Facebook Logo" />
                        <a href="#"><p>Facebook</p></a>
                    </li>
                    <li>
                        <img src="twitter.png" alt="Twitter Logo" />
                        <a href="#"><p>Twitter</p></a>
                    </li>
                    <li>
                        <img src="telegram.png" alt="Telegram Logo" />
                        <a href="#"><p>Telegram</p></a>
                    </li>
                </ul>
            </footer>
        </div>
    </div>
</body>
</html>
* {
  margin: 0;
  padding: 0;
}
 
body {
  background-color: #eff1f2;
  font-family: sans-serif;
}
 
.content {
  grid-area: content;
}
 
.sidebar {
  grid-area: sidebar;
  background: linear-gradient(
    to right,
    rgba(200, 107, 142, 1),
    rgba(218, 105, 250, 1),
    rgba(110, 125, 253, 1)
  );
  justify-content: center;
}
 
.footer {
  grid-area: footer;
  background: white;
}
 
.container {
  font-size: 1.5em;
  width: 100%;
  height: 100;
  height: 100vh;
  display: grid;
  grid-template-areas: 'sidebar' 'content' 'footer';
  grid-template-columns: 1fr;
  grid-template-rows: 130px 800px 250px;
}
 
.content,
.sidebar,
.footer {
  padding: 1em;
}
 
nav ul {
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: space-between;
  text-align: center;
}
 
nav li {
  list-style: none;
  padding: 1em 0;
}
 
nav li a {
  color: white;
  font-weight: 700;
  opacity: 0.6;
  text-decoration: none;
  transition: 0.3s;
}
 
nav li a:hover {
  opacity: 1;
}
 
.hero {
  max-width: 90 px;
  margin: 0 auto;
  text-align: center;
}
 
.hero img {
  width: 200px;
}
 
.hero h1 {
  font-size: 2em;
  font-weight: 300;
  color: #373046;
}
 
.hero p {
  font-weight: 300;
  line-height: 1.3em;
  color: #98abad;
}
 
.action-btn {
  display: inline-block;
  text-decoration: none;
  color: white;
  font-weight: 700;
  background: #567bfb;
  padding: 0.5em 2em;
  border-radius: 60px;
  margin: 1em 0;
  transition: 0.3s;
}
 
footer ul {
  max-width: 640px;
  margin: 2em auto;
  padding: 0;
  text-align: center;
  display: flex;
  flex-direction: row;
}
 
footer ul li {
  list-style: none;
  align-self: flex-end;
}
 
footer ul li a {
  text-decoration: none;
  color: #c1c6ce;
}
 
footer ul li img {
  width: 30%;
}
 
footer p {
  font-size: 0.8em;
}
 
@media (min-width: 1040px) {
  .container {
    grid-template-areas: 'sidebar content' 'sidebar footer';
    grid-template-rows: 1fr auto;
    grid-template-columns: 300px 1f;
  }
 
  nav ul {
    display: flex;
    justify-content: space-between;
    flex-direction: column;
  }
 
  .sidebar {
    background: linear-gradient(
      rgba(200, 107, 142, 1),
      rgba(218, 105, 250, 1),
      rgba(110, 125, 253, 1)
    );
    padding-top: 10em;
  }
 
  .hero {
    text-align: left;
    margin: 7em 0;
  }
 
  .hero img {
    width: 200px;
    float: right;
  }
 
  .hero h1 {
    font-size: 3em;
  }
 
  .hero p {
    width: 60%;
  }
 
  footer ul {
    max-width: 900px;
    margin: 0 auto;
    padding: 1em 0;
  }
 
  footer ul li a img {
    width: 20%;
  }
}
