# 🃏 Card Flip Memory Game

A fun and interactive **Card Flip Memory Game** built with vanilla HTML, CSS, and JavaScript — containerized with **Docker** and deployed on an **AWS EC2 instance** using **Rocky Linux 8**.

![Preview Screenshot](https://github.com/shubham-jain-dev/docker-web-game/raw/main/images/preview.png) <!-- Replace with actual screenshot if available -->

---

## 🚀 Features

- Flip cards to find matching pairs 🎯
- Simple, clean UI with smooth animations
- Responsive design
- Dockerized for easy deployment
- Hosted on an AWS EC2 instance

---

## 💻 Tech Stack

- HTML / CSS / JavaScript
- Apache HTTP Server
- Docker
- Rocky Linux 8
- AWS EC2

---

## 📁 Project Structure
. ├── Dockerfile # Docker configuration 
  ├── index.html # Main game UI 
  ├── style.css # Styles and animations 
  ├── script.js # Game logic 
  
---

## 🐳 Run the Game Using Docker

### 1. Clone the Repository
```bash
git clone https://github.com/shubham-jain-dev/docker-web-game.git
cd docker-web-game
2. Build the Docker Image
bash
Copy
Edit
docker build -t card-flip-game .
3. Run the Container
bash
Copy
Edit
docker run -d -p 80:80 card-flip-game
Now open http://localhost in your browser and play the game!

🌐 Deploying to AWS EC2
Launch an EC2 instance (Amazon Linux / Rocky Linux 8)

SSH into the instance:

bash
Copy
Edit
ssh -i your-key.pem ec2-user@your-ec2-ip
Install Docker:

bash
Copy
Edit
sudo dnf install -y docker
sudo systemctl start docker
sudo systemctl enable docker
sudo usermod -aG docker ec2-user
Clone, build, and run the container:

bash
Copy
Edit
git clone https://github.com/shubham-jain-dev/docker-web-game.git
cd docker-web-game
docker build -t card-flip-game .
docker run -d -p 80:80 card-flip-game
Access the game at:
http://your-ec2-public-ip

🙌 Acknowledgments
Created with ❤️ by Shubham Jain

