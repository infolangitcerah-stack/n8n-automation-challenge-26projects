
# 🌞 n8nProject 01: Daily Motivation Bot

## 🎯 Problem
We often start our mornings without focus or motivation.  
This project automates a **daily inspirational quote** delivered directly to your Telegram.

## 🚀 Solution
- Trigger every morning at **8:00 AM** using the Cron node  
- Fetch a random quote from **ZenQuotes API**  
- Send the formatted message to **multiple Telegram recipients**

## 🛠️ Workflow Steps
1. **Cron Node** → runs at 8:00 AM daily  
2. **HTTP Request Node** → fetches random quote from `https://zenquotes.io/api/random`  
3. **Set Node** → stores multiple chat IDs (recipients)  
4. **Telegram Node** → sends the same quote to each recipient  

## 📸 Workflow Screenshot
![Workflow Screenshot](./workflow.png)
![n8n01Challenge1](https://github.com/user-attachments/assets/80bf995c-02d3-4f8c-bdd6-2d3121886331)


## 📲 Telegram Output
![Telegram Output](./telegram-output.png)
![n8n01Challenge2](https://github.com/user-attachments/assets/d2801fd3-bda8-4b15-a75d-39a9e230ac5b)

---

## 🔧 Setup Instructions
1. Create a bot with **@BotFather** in Telegram and save the API token  
2. Get your **chat ID** (or group ID) via [@userinfobot](https://t.me/userinfobot)  
3. Add multiple chat IDs in the **Set node**  
4. Configure the **Telegram node** with your bot credentials  
5. Activate workflow — enjoy your daily inspiration!  

---

## ✅ Example Output

🌞 Good Morning!
💡 The best way to get started is to quit talking and begin doing. — Walt Disney
