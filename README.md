# DSAForgebot-Telegram DSA Practice Bot

**DSAForgebot** is a smart, Java-based Telegram bot that recommends LeetCode DSA (Data Structures & Algorithms) problems based on user-selected difficulty and topic. It tracks your progress, ensures non-repetitive suggestions, and streamlines your problem-solving workflow — all through a clean, chat-based interface.

## 🚀 Features

- 📚 Intelligent problem recommendation based on topic and difficulty
- ⌨️ Inline keyboard interaction and Telegram command support
- 📈 Persistent progress tracking using MySQL
- ✅ "Done" command to move to the next relevant problem
- 🔐 Per-user session handling for isolation and continuity
- 🧩 Built with scalability and versioning in mind

## 🧠 Tech Stack

- **Language:** Java  
- **Database:** MySQL  
- **Bot API:** TelegramBots Java SDK  
- **Build Tool:** Maven / Gradle  
- **Version Control:** Git & GitHub

## Project Structure
DSAForgebot-v2.1/
├── src/
│   ├── main/
│   │   ├── bot/                # Telegram bot logic
│   │   ├── handlers/           # Command handlers
│   │   ├── models/             # User, Problem POJOs
│   │   ├── db/                 # DBConnection + SQL logic
│   │   ├── util/               # Utility and helper functions
│   │   └── Main.java           # Bot launcher
├── resources/
│   └── questions.sql           # LeetCode question dump
├── README.md
└── pom.xml                     # Maven project config


⚙️ Core Commands
Command	Description
/start	Initializes or resets the bot for user
/topic	Lets user choose a topic from a menu
/level	Choose difficulty after topic
done	Confirms question solved, loads next
/stats	Shows solved count and streaks
/help	Shows instructions



## ⚙️ Setup Instructions

### ✅ Prerequisites

- Java 11 or higher  
- MySQL server (local or remote)  
- Telegram bot token from [@BotFather](https://t.me/botfather)  
- Maven or Gradle (your choice)

### 🚀 Steps to Run

```bash
# 1. Clone the repository
git clone https://github.com/your-username/dsa-forgebot.git
cd dsa-forgebot

# 2. Set up your environment
# - Configure DB credentials
# - Add Telegram bot token in a config file or environment variable

# 3. Build and Run
mvn clean install
java -jar target/dsa-forgebot.jar



