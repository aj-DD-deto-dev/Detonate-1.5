# Detonate Multiplayer Game

## Installation Instructions

1. **Clone the repository** to your local machine:
   ```bash
   git clone https://github.com/aj-DD-deto-dev/Detonate-1.5.git
   ```

2. **Navigate to the project directory**:
   ```bash
   cd Detonate-1.5
   ```

3. **Install dependencies**:
   Make sure you have [Node.js](https://nodejs.org/) installed, then run:
   ```bash
   npm install
   ```

4. **Set up the environment variables**:
   Create a `.env` file in the root directory and set the required variables (refer to `.env.example` for guidance).

5. **Build the project**:
   ```bash
   npm run build
   ```

6. **Start the server**:
   ```bash
   npm start
   ```

## Deployment Instructions

1. **Choose a cloud provider** (e.g., AWS, Azure, Digital Ocean).

2. **Set up a server** based on your chosen provider's instructions.

3. **Upload the project files** to the server using `scp` or an FTP client.

4. **Install necessary software** (Node.js, npm) on the server if not already installed.

5. **Configure the server to run your application** using a process manager like PM2:
   ```bash
   npm install -g pm2
   pm2 start npm --name "detonate" -- start
   ```

6. **Set up a reverse proxy** (e.g., using Nginx) to route requests to your application.

7. **Secure your application** with HTTPS (Let’s Encrypt can be used for free SSL certificates).

## Troubleshooting

- If you encounter issues, check the logs with:
  ```bash
  pm2 logs detonate
  ```
- Common issues include incorrect environment variables or dependency problems. Double-check your setup and consult the issues section on GitHub if needed.

## Additional Resources

- [Detonate GitHub Repository](https://github.com/aj-DD-deto-dev/Detonate-1.5)
- [Node.js Documentation](https://nodejs.org/docs/)
- [PM2 Documentation](https://pm2.keymetrics.io/docs/usage/quick-start/)