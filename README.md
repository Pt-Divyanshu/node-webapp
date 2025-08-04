# 🚀 Node.js Web App with CI/CD Pipeline

This is a simple Node.js web application with a fully automated CI/CD pipeline using **GitHub Actions** and **Docker Hub**. Whenever changes are pushed to the `main` branch, the workflow:

1. Installs dependencies
2. Runs tests
3. Builds a Docker image
4. Pushes the image to Docker Hub

---

## 📁 Project Structure

node-webapp/
├── .github/
│ └── workflows/
│ └── main.yml # GitHub Actions workflow
├── Dockerfile # Docker build instructions
├── app.js # Main application file
├── package.json # NPM configuration
└── README.md # Project documentation


---

## 🧰 Technologies Used

- **Node.js** (Express)
- **GitHub Actions** (CI/CD)
- **Docker** (Containerization)
- **Docker Hub** (Image registry)

---

## ▶️ Running the App Locally

```bash
git clone https://github.com/your-username/node-webapp.git
cd node-webapp
npm install
npm start

App will be available at http://localhost:3000.

Docker

🔨 Build Docker Image

docker build -t your-dockerhub-username/node-webapp .

🚀 Run the Container

docker run -p 3000:3000 your-dockerhub-username/node-webapp

🔄 GitHub Actions Workflow

The CI/CD workflow is defined in .github/workflows/main.yml.
On Every Push to main Branch:

    Runs npm install and npm test

    Builds the Docker image

    Pushes the image to Docker Hub (your-dockerhub-username/node-webapp:latest)

🔐 GitHub Repository Secrets

Set the following secrets in your repository settings:
Secret Name Description
DOCKER_USERNAME Your Docker Hub username
DOCKER_PASSWORD Docker Hub password or token


📦 Example API Endpoint

Once deployed (locally or via Docker), visit:

GET http://localhost:3000/

Response:

Hello from Node.js!


🛠️ Future Enhancements

    Add unit and integration tests

    Add deployment step to cloud/VPS

    Use Docker tags based on git commit or versioning

📄 License

MIT License – do whatever you want, but don’t blame me if it breaks 🙂


🤝 Contributing

Feel free to fork this repo and submit PRs!


Let me know if you'd like the README to include **badges** (build status, Docker pulls, etc.) or **deployment instructions to a specific platform** like AWS, DigitalOcean, or Render.
