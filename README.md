# IronClaw WordPress Assistant

A secure, open-source tool for IronClaw users to update their WordPress sites via API — without exposing secrets.

## 🛠 Features
- OAuth2 login (no passwords)
- No hardcoded keys
- Works with WordPress.com and self-hosted sites
- Full audit trail (no data stored)

## 📦 How to Use
1. Register a new app at [https://developer.wordpress.com/apps](https://developer.wordpress.com/apps)
2. Copy your **Client ID** and **Client Secret**
3. Run:
   ```bash
   # Install via IronClaw
   tool_install name=ironclaw-wordpress-assistant
   tool_auth name=wordpress

create_job title="Update Post" description="Add new event" credentials='{"wordpress_api_key": "wordpress"}' mode="worker"
