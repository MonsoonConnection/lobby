# lobby
The unified portal and application delivery platform for a pure off-the-cloud ecosystem. A containerized entry point designed specifically for local self-hosted homelabs and home-office solutions.

## Quick Start

### 1. Clone the repository
```bash
git clone https://github.com/MonsoonConnection/lobby.git
cd lobby
```

### 2. Configure Environment
Copy the example environment file and adjust it to your needs:
```bash
cp .env.example .env  # Edit .env with your local domain and settings
```

### 3. Deploy the stack
Start all services in detached mode:
```bash
docker compose up -d
```
That’s it! Your Lobby services should now be running.

### 4. Access the Lobby
Open your browser and navigate to: `http://lobby.local` (or the domain you configured in your .env)

#### Local DNS Configuration: ####
Since this is an off-the-cloud local setup, you need to map your domain to the server's IP address. 

**Windows:** Edit `C:\Windows\System32\drivers\etc\hosts` (as Admin)
 **Mac/Linux:** Edit `/etc/hosts` (as sudo) Add the following line:
  ```text
   192.168.x.x lobby.local (or the domain you configured in your .env)
