*Title: Deploy A Simple HTML Web Page Using Nginx*

🚀 *Project Overview*:  
This project demonstrates how to deploy a simple HTML webpage using Nginx inside a Docker container. It involves setting up an HTML file, hosting it in a local directory, and serving it via Nginx by exposing it on port 8080.

🔧 *What You'll Learn*:
- Setting up a local directory to host an HTML file.
- Creating and editing an index.html file.
- Running an Nginx container with Docker and exposing it to the web.
- Serving a webpage via Nginx and making real-time changes visible.

📖 *Step-by-Step Guide*:
1. *Create a Host Directory*:
   - Use mkdir to create a directory named website for your HTML files.

2. *Create an HTML File*:
   - Inside the directory, create an index.html file with the following updated HTML code:
     html
     <!doctype html>
     <html lang="en">
     <head>
       <meta charset="utf-8">
       <title>Home page</title>
     </head>
     <body>
       <h1>Hello from Hossam Farhoud</h1>
       <p>Regards,</p>
       <p>Hossam Farhoud</p>
       <a href="https://www.linkedin.com/in/hossam-farhoud/" target="_blank">Connect with Me</a>
     </body>
     </html>
     

3. *Run the Nginx Docker Container*:
   - Run an Nginx container with the following command:
     bash
     docker run -it -d --name web -p 8080:80 -v ~/website:/usr/share/nginx/html nginx
     

4. *Access the Webpage*:
   - Open your browser and go to localhost:8080 to view the HTML webpage.
   - Any changes made to the index.html file will reflect immediately upon saving.

🔗 *Why Use Nginx with Docker?*:
- *Efficiency*: Simple and quick setup for serving static files.
- *Portability*: Docker allows easy deployment of Nginx without manual installation.
- *Live Updates*: Real-time changes to HTML files are instantly visible.

🛠 *Tools and Technologies*:
- Docker
- Nginx
- HTML

📂 *GitHub Repository*:  
Check out the full project and code on GitHub: [Deploy A Simple HTML Web Page Using Nginx](https://github.com/hossamfarhoud/Deploy-A-Simple-HTML-Web-Page-Using-Nginx#deploy-a-simple-html-web-page-using-nginx)

---

Hashtags: #Docker #Nginx #WebDevelopment #HTML #CloudComputing #Containers #DevOps
