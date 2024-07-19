# Hosting on VPS Server

## Setup Hosting

1. Update and upgrade the system:
    ```bash
    sudo apt update
    sudo apt upgrade
    ```

2. Install Node Version Manager (NVM):
    ```bash
    curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
    ```

3. Install Node.js and NVM:
    ```bash
    apt install nodejs
    nvm install --lts
    node -v
    ```

4. Install Git and GitHub CLI:
    ```bash
    sudo apt install git
    sudo apt install gh
    gh auth login
    ```

5. Install global npm packages:
    ```bash
    npm i -g pnpm  # For installing modules in node
    npm i -g pm2   # To run our server 24x7
    ```

6. Install Nginx and Certbot:
    ```bash
    sudo apt install nginx
    sudo apt-get install certbot python3-certbot-nginx  # For requesting the SSL Certificate
    ```

### Reminder

After every new download, please run the following commands:
```bash
sudo apt update
sudo apt upgrade
