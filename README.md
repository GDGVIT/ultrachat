<p align="center">
<a href="https://dscvit.com">
	<img width="400" src="https://user-images.githubusercontent.com/56252312/159312411-58410727-3933-4224-b43e-4e9b627838a3.png#gh-light-mode-only" alt="GDSC VIT"/>
</a>
	<h2 align="center"> UltraChat </h2>
	<h4 align="center"> UltraChat is a powerful Discord bot designed to enhance productivity in servers by providing chat summarization and management. </h4>
</p>

---

[![Join Us](https://img.shields.io/badge/Join%20Us-Developer%20Student%20Clubs-red)](https://dsc.community.dev/vellore-institute-of-technology/)
[![Discord Chat](https://img.shields.io/discord/760928671698649098.svg)](https://discord.gg/498KVdSKWR)

This project consists of two main components:
- [UltraChat Bot](https://github.com/GDGVIT/ultra-chat-bot) - Discord bot for chat summarization
- [UltraChat Backend](https://github.com/GDGVIT/ultra-chat-backend) - Golang backend service

## Discord Bot

### Features
- Discord OAuth2 Integration
- Chat summarization capabilities
- Interactive commands via `!help`
- Support for multiple API integrations:
  - HuggingFace API
  - Groq API
  - Discord API
  - Cohere API

### Bot Installation

1. Clone the repository:
```bash
git clone https://github.com/GDGVIT/ultra-chat-bot.git
cd ultra-chat-bot
```

2. Set up environment variables:
   - Copy `.env.example` and rename to `.env`
   - Add all required API keys
   - Configure Discord bot token

3. Create and activate virtual environment:

**Windows:**
```bash
python -m venv venv
.\venv\Scripts\activate
```

**Linux and MacOS:**
```bash
python -m venv venv
source venv/bin/activate
```

4. Install dependencies:
```bash
pip install -r requirements.txt
```

5. Run the bot:
```bash
python app.py
```

## Backend Service

### Backend Features
- JWT based authentication
- User profile management
- Summary management:
  - Create and retrieve chat summaries
  - Update existing summaries
  - Delete summaries
  - Private/Public summary options

### Backend Installation

1. Clone the backend repository:
```bash
git clone https://github.com/GDGVIT/ultra-chat-backend.git
```

2. Install Go dependencies:
```bash
go mod download
```

3. Set required environment variables:
```bash
export PORT=5001
export MONGODB_URI=your_mongodb_uri
export CLIENT_ID=your_discord_client_id
export CLIENT_SECRET=your_discord_client_secret
export REDIRECT_URI=your_redirect_uri
```

4. Run the server:
```bash
go run main.go
```

### Docker Setup

If you prefer using Docker:

1. Ensure all credentials are in `.env`
2. Build and run using Docker Compose:
```bash
docker-compose build
docker-compose up
```

## API Documentation

View the complete [Postman API Documentation](https://github.com/DevloperAmanSingh/ultra-chat-backend/blob/main/postman.json) for detailed endpoint information.

Key endpoints:
- `POST /create-summary` - Create new chat summary
- `GET /summarizer` - Get user summaries
- `PUT /update-summary` - Update existing summary
- `DELETE /delete-summary` - Delete summary
- `GET /is_authenticated` - Check authentication status

## Contributors

<table>
	<tr align="center">
		<td>
		Noel Alex
		<p align="center">
			<img src = "https://avatars.githubusercontent.com/u/79050483?v=4" width="150" height="150" alt="Noel Alex">
		</p>
			<p align="center">
				<a href = "https://github.com/Noel-alex">
					<img src = "http://www.iconninja.com/files/241/825/211/round-collaboration-social-github-code-circle-network-icon.svg" width="36" height = "36" alt="GitHub"/>
				</a>
				<a href = "https://www.linkedin.com/in/noel-alex-b1731128b/">
					<img src = "http://www.iconninja.com/files/863/607/751/network-linkedin-social-connection-circular-circle-media-icon.svg" width="36" height="36" alt="LinkedIn"/>
				</a>
			</p>
		</td>
		<td>
		Sidhant Srivastav
		<p align="center">
			<img src = "https://avatars.githubusercontent.com/u/66166455?v=4" width="150" height="150" alt="Sidhant Srivastav">
		</p>
			<p align="center">
				<a href = "https://github.com/sidhant-sriv">
					<img src = "http://www.iconninja.com/files/241/825/211/round-collaboration-social-github-code-circle-network-icon.svg" width="36" height = "36" alt="GitHub"/>
				</a>
				<a href = "https://www.linkedin.com/in/sidhant-srivastava-41803620b/">
					<img src = "http://www.iconninja.com/files/863/607/751/network-linkedin-social-connection-circular-circle-media-icon.svg" width="36" height="36" alt="LinkedIn"/>
				</a>
			</p>
		</td>
		<td>
		Aman Singh
		<p align="center">
			<img src = "https://avatars.githubusercontent.com/u/80804989?v=4" width="150" height="150" alt="Aman Singh">
		</p>
			<p align="center">
				<a href = "https://github.com/DevloperAmanSingh">
					<img src = "http://www.iconninja.com/files/241/825/211/round-collaboration-social-github-code-circle-network-icon.svg" width="36" height = "36" alt="GitHub"/>
				</a>
				<a href = "https://www.linkedin.com/in/amansingh2112">
					<img src = "http://www.iconninja.com/files/863/607/751/network-linkedin-social-connection-circular-circle-media-icon.svg" width="36" height="36" alt="LinkedIn"/>
				</a>
			</p>
		</td>
	</tr>
</table>

<p align="center">
	Made with ❤ by <a href="https://dscvit.com">GDSC-VIT</a>
</p>
