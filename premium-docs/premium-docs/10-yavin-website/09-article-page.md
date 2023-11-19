# Article Page

Now we are going to create an inner page for this site. This is the page that will show when someone clicks on one of the profile links.

Create a new page in the root called `article.html`. We need the outter layout from the `index.html` page. Get the `head` tags and everything in them and in the body, get the `navbar`, `footer` and the bring to top button. Paste all of this in the `article.html` page.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link
      href="https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,400;0,600;0,700;1,400&display=swap"
      rel="stylesheet"
    />
    <link rel="stylesheet" href="css/font-awesome.css" />
    <link rel="stylesheet" href="css/bootstrap.css" />
    <link rel="stylesheet" href="css/styles.css" />
    <link rel="icon" href="images/favicon.png" />
    <title>Yavin Office Design</title>
  </head>
  <body>
    <!-- Navigation -->
    <nav class="navbar navbar-expand-lg sticky-top navbar-light">
      <div class="container">
        <a class="navbar-brand" href="index.html">
          <img src="images/logo.svg" alt="" width="124" />
        </a>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarNavDropdown"
          aria-controls="navbarNavDropdown"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNavDropdown">
          <ul class="navbar-nav ms-auto">
            <li class="nav-item">
              <a class="nav-link" aria-current="page" href="index.html">Home</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#details">Details</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#services">Services</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#projects">Projects</a>
            </li>
            <li class="nav-item">
              <a
                class="nav-link btn btn-outline-secondary px-4 mx-4"
                href="#contact"
                >Contact Us</a
              >
            </li>
          </ul>
        </div>
      </div>
    </nav>

    <!-- Footer -->
    <div class="footer bg-light py-6">
      <div class="container">
        <div class="row">
          <div class="col-md-4 my-3">
            <h6>About Yavin</h6>
            <p class="p-small">
              He oppose at thrown desire of no. Announcing impression unaffected
              day his are unreserved indulgence. Him hard find read are you
            </p>
          </div>
          <div class="col-md-4 my-3">
            <h6>Links</h6>
            <ul class="list-unstyled li-space-lg p-small">
              <li>
                Important: <a href="#">Terms & Conditions</a>,
                <a href="#">Privacy Policy</a>
              </li>
              <li>
                Useful: <a href="#">Colorpicker</a>,
                <a href="#">Icon Library</a>, <a href="#">Illustrations</a>
              </li>
              <li>
                Menu: <a href="#header">Home</a>,
                <a href="#details">Details</a>,
                <a href="#services">Services</a>, <a href="#contact">Contact</a>
              </li>
            </ul>
          </div>
          <div class="col-md-4 my-3">
            <div class="mb-4">
              <a href="#" class="text-decoration-none">
                <i class="fab fa-facebook fa-3x text-dark mx-2"></i>
              </a>
              <a href="#" class="text-decoration-none">
                <i class="fab fa-twitter fa-3x text-dark mx-2"></i>
              </a>
              <a href="#" class="text-decoration-none">
                <i class="fab fa-instagram fa-3x text-dark mx-2"></i>
              </a>
              <a href="#" class="text-decoration-none">
                <i class="fab fa-pinterest fa-3x text-dark mx-2"></i>
              </a>
            </div>
            <p class="p-small">
              We would love to hear from you
              <a href="mailto:contact@site.com"
                ><strong>contact@site.com</strong></a
              >
            </p>
          </div>
        </div>
      </div>
    </div>

    <button id="to-top" class="to-top-btn">
      <img src="images/up-arrow.png" alt="" />
    </button>

    <script src="js/bootstrap.bundle.js"></script>
    <script src="js/script.js"></script>
  </body>
</html>
```

This is basically your starter for any other pages that you want to create, so you may want to just save this code somewhere so you can copy and paste it later.

## Header & Image

We have a simple header with some text and an image. Add the following html:

```html
 <!-- Header -->
<header class="bg-light py-6">
  <div class="container">
    <h1>Article Details</h1>
  </div>
</header>

<!-- Image -->
<section>
  <div class="container">
    <img src="images/article-details-large.jpg" alt="" class="w-100 my-6" />
  </div>
</section>
```

## Basic Text

Next is just some basic text. Add the following html:

```html
<!-- Basic Text -->
    <section class="pt-4">
      <div class="container">
        <div class="row">
          <div class="col-lg-10 offset-lg-1">
            <p>
              Lorem ipsum dolor sit amet consectetur, adipisicing elit. Placeat
              eligendi, labore pariatur repudiandae consectetur totam eum
              voluptatem blanditiis nulla architecto fugiat tempore obcaecati
              molestias porro! Nisi ullam inventore eveniet quas.
            </p>

            <p class="mb-4">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio
              architecto assumenda cum nemo omnis velit nobis, nihil veniam esse
              ratione.
            </p>

            <h2 class="mb-3">Advantages of working with this company</h2>

            <p>
              Lorem ipsum dolor sit amet consectetur, adipisicing elit. Placeat
              eligendi, labore pariatur repudiandae consectetur totam eum
              voluptatem blanditiis nulla architecto fugiat tempore obcaecati
              molestias porro! Nisi ullam inventore eveniet quas.
            </p>

            <p class="mb-4">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio
              architecto assumenda cum nemo omnis velit nobis, nihil veniam esse
              ratione.
            </p>
          </div>
        </div>
      </div>
    </section>
```

Here, we are making the column 10 columns wide, instead of the full 12. We are also using the `offset-xl-1` class to center the column.

## Cards

Next we have some cards. Add the following html:

```html
<!-- Cards -->
    <section class="my-4">
      <div class="container">
        <div class="row">
          <div class="col-md-4">
            <div class="card">
              <div class="card-body">
                <h5>
                  <i class="fas fa-check text-secondary"></i> High Quality
                  Service
                </h5>
                <p>
                  Lorem ipsum dolor sit amet consectetur adipisicing elit. Quam
                  culpa provident, aliquam officia expedita recusandae!
                </p>
              </div>
            </div>
          </div>
          <div class="col-md-4">
            <div class="card my-3">
              <div class="card-body">
                <h5>
                  <i class="fas fa-check text-secondary"></i> Prompt Timely
                  Service
                </h5>
                <p>
                  Lorem ipsum dolor sit amet consectetur adipisicing elit. Quam
                  culpa provident, aliquam officia expedita recusandae!
                </p>
              </div>
            </div>
          </div>
          <div class="col-md-4">
            <div class="card">
              <div class="card-body">
                <h5>
                  <i class="fas fa-check text-secondary"></i> Skilled Team
                  Involved
                </h5>
                <p>
                  Lorem ipsum dolor sit amet consectetur adipisicing elit. Quam
                  culpa provident, aliquam officia expedita recusandae!
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
```

## Gray Box

Finally, we just have some text in a gray box. Add the following html:

```html
<!-- Gray Box -->
    <section class="my-5">
      <div class="row">
        <div class="col-lg-8 offset-lg-2">
          <div class="card bg-light rounded-0 border-0 fs-6">
            <div class="card-body p-4">
              <h3>We Know What Our Customers Want</h3>
              <p>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit.
                Voluptatum at optio quod tempora cupiditate fugit dolores quam,
                fuga ipsam aliquid rerum provident. Possimus, velit voluptatum?
                Magnam hic ab doloremque ipsam?
              </p>
            </div>
          </div>
        </div>
      </div>
    </section>
```

Here, we are only making the width of the column 8 columns wide, instead of the full 12. We are also using the `offset-xl-2` class to center the column.

That's it! We have completed the Yavin website. Feel free to change and add things to make it your own.