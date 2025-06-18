[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&width=435&lines=Welcome+To+Launch+Airdrop)](https://git.io/typing-svg)

# Voyager CraftWorld Auto Bot

This bot automatically handles daily login, quest claiming, and chest spinning for multiple wallets on the Voyager CraftWorld platform.

## Features

- Multi-wallet support - Process multiple wallets automatically
- Daily quest automation - Auto-claim ready quests
- Chest spinning - Auto-spin daily free chests and coin chests
- Proxy support - Use HTTP/HTTPS/SOCKS4/SOCKS5 proxies for each wallet
- Daily reset countdown - Automatically waits for next daily reset
- Session management - Handle authentication and sessions automatically

## Getting Started

### Register Your Account
First, create your Voyager CraftWorld account :
**[Register Here](https://voyager.preview.craft-world.gg)**

## Installation

### Clone the Repository
```bash
git clone https://github.com/LaunchAirdrop/voyager.git
cd voyager
```

Install Dependencies
```bash
npm install 
```
or
```bash
npm install dotenv axios ethers siwe https-proxy-agent http-proxy-agent socks-proxy-agent crypto-js
```

Edit and input Private Key:
```bash
nano .env
```

Run the script
```bash
node index.js
```

### Proxy Setup (Optional)
```bash
nano proxy.txt
```
**Proxy Format Examples:**
```txt
# HTTPS Proxies  
https://username:password@proxy.example.com:8080
```

### The bot will:
1. Authentication - Signs in to each wallet using SIWE (Sign-In with Ethereum)
2. Daily Login - Completes daily login quest
3. Quest Claiming - Automatically claims all ready quests
4. Chest Spinning - Opens available daily chests:
   - Daily Chest (Free)
   - Sturdy Chest (Coin)
5. Daily Loop - Waits for next daily reset and repeats

## ⚠️ Important Notes

- **Private Key Security**: Never share your private keys. Keep your `.env` file secure.
- **Rate Limiting**: The bot includes delays between requests to avoid rate limiting.
- **Daily Reset**: The bot automatically waits for the next daily reset (00:00 UTC).
- **Proxy Testing**: All proxies are tested before use. Only working proxies are utilized.

## Security Best Practices

1. **Use Dedicated Wallets**: Create separate wallets specifically for this bot.
2. **Limited Funds**: Only keep minimal funds needed for transactions.
3. **Secure Environment**: Run the bot on a secure server or local machine.
4. **Regular Updates**: Keep the bot updated with the latest version.

### Common Issues

**"No private keys found"**
- Make sure your `.env` file exists and contains `PRIVATE_KEY_1=...` format

**"Proxy connection failed"**
- Verify your proxy credentials and format in `proxies.txt`
- The bot will work without proxies if none are available

**"Authentication failed"**
- Check if your private key is valid
- Ensure your wallet has some ETH for gas fees

**"Rate limit reached"**
- The bot includes automatic delays, but you can increase them if needed
- Consider using fewer wallets or longer delays

## Max 10 wallet


## 📄 License

This project is for educational purposes. Use at your own risk.

---
 **Don't forget to star this repository if it helped you!**
