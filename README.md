<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Example Website Header</title>
<STYLE>
    * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background: linear-gradient(to bottom, #e0f7fa, #f0f4f8);
}

header {
    background: linear-gradient(to right, #3b8ef4, #4fa3f7);
    color: white;
    padding: 20px;
    text-align: center;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

nav {
    margin-bottom: 20px;
}

.nav-btn {
    background-color: #4fa3f7;
    color: white;
    border: none;
    padding: 10px 20px;
    margin: 5px;
    cursor: pointer;
    border-radius: 5px;
    font-size: 16px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.nav-btn:hover {
    background-color: #2976cc;
    box-shadow: 0 6px 8px rgba(0, 0, 0, 0.2);
}

h1 {
    margin-top: 10px;
}

main {
    display: flex;
    justify-content: space-between;
    padding: 20px;
}

.contact-form, .intro-video {
    background: linear-gradient(to right, #ffed6b, #ffda5c);
    padding: 20px;
    border-radius: 10px;
    width: 48%;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
}

.contact-form h2, .intro-video h2 {
    margin-bottom: 20px;
}

.contact-form label {
    display: block;
    margin-bottom: 5px;
    font-weight: bold;
}

.contact-form input, .contact-form textarea {
    width: 100%;
    padding: 10px;
    margin-bottom: 15px;
    border-radius: 5px;
    border: 1px solid #ccc;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.05);
}

.contact-form textarea {
    resize: vertical;
    height: 150px;
}
.submit-btn {
    background: linear-gradient(to right, #ff4c4c, #44c767);  /* Gradient from red (#ff4c4c) to green (#44c767) */
    color: white;
    width: 70%;
    padding: 10px 20px;
    border: none;
    border-radius: 30px;  /* Rounded corners */
    cursor: pointer;
    font-size: 16px;
    text-align: center;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.2);  /* Subtle shadow */
   
}
.submit-btn:hover {
    background: linear-gradient(to right, #44c767, #ff4c4c);  /* Reverse gradient on hover */
    box-shadow: 0 6px 8px rgba(0, 0, 0, 0.3);  /* Stronger shadow on hover */
}


.intro-video .video-container {
    display: flex;
    justify-content: center;
}

.video-container video {
    border-radius: 10px;
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
}

@media screen and (max-width: 768px) {
    main {
        flex-direction: column;
        align-items: center;
    }

    .contact-form, .intro-video {
        width: 80%;
        margin-bottom: 20px;
    }
}

@media screen and (max-width: 768px) {
    main {
        flex-direction: column;
        align-items: center;
    }

    .contact-form, .intro-video {
        width: 80%;
        margin-bottom: 20px;
    }
}

</STYLE>
</head>
<body>
    <header>
        <nav>
            <button class="nav-btn">Home</button>
            <button class="nav-btn">About</button>
            <button class="nav-btn">Contact</button>
        </nav>
        <h1>Example Website Header</h1>
    </header>

    <main>
        <section class="contact-form">
            <h2>Contact Form</h2>
            <form action="#" method="post">
                <label for="name">Name</label>
                <input type="text" id="name" name="name" placeholder="Enter your name" required>

                <label for="email">Email</label>
                <input type="email" id="email" name="email" placeholder="Enter your email" required>

                <label for="message">Message</label>
                <textarea id="message" name="message" placeholder="Write your message" required></textarea>

                <button type="submit" class="submit-btn">Submit</button>
            </form>
        </section>

        <section class="intro-video">
            <h2>Intro Video</h2>
            <div class="video-container">
                <video width="320" height="240" controls>
                    <source src="your-video.mp4" type="video/mp4">
                    Your browser does not support the video tag.
                </video>
            </div>
        </section>
    </main>
</body>
</html>
