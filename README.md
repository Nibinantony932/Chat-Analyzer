# 🪄 CHAT-ANALYZER

A powerful WhatsApp chat analyzer built with Streamlit that helps you extract meaningful insights from your WhatsApp conversations.

---

## 📋 Table of Contents

- [Features](#features)
- [Demo](#demo)
- [Installation](#installation)
- [How to Use](#how-to-use)
- [Exporting WhatsApp Chats](#exporting-whatsapp-chats)
- [What You'll Get](#what-youll-get)
- [Technical Details](#technical-details)
- [Contributors](#contributors)
- [License](#license)

---

## ✨ Features

- **📊 Interactive Visualizations**: Beautiful charts showing message distribution across users
- **👑 Most Active User Detection**: Instantly identifies who sends the most messages
- **📝 Word Frequency Analysis**: Discovers the most commonly used words (excluding common stop words and media)
- **🕒 Timeline Analysis**: Visualizes message patterns over time
- **⚡ Fast Processing**: Efficient parsing algorithm handles large chat files
- **🎨 Modern UI**: Clean, dark-themed interface with smooth animations

---

## 🌐 Demo

You can access the live application at:
**[Your Streamlit App Link Here]**

Or run it locally by following the installation instructions below.

---

## 🚀 Installation

### Prerequisites

- Python 3.7 or higher
- pip (Python package manager)

### Step 1: Clone or Download the Repository

Download the project files to your local machine.

### Step 2: Install Required Dependencies

Open your terminal/command prompt in the project directory and run:

```bash
pip install streamlit plotly
```

### Step 3: Run the Application

```bash
streamlit run app.py
```

The application will automatically open in your default web browser at `https://chat-analyzer-00.streamlit.app/`

---

## 📖 How to Use

### 1. Export Your WhatsApp Chat

#### On Android:
1. Open the WhatsApp chat you want to analyze
2. Tap the three dots (⋮) in the top right corner
3. Select **More** → **Export chat**
4. Choose **Without media**
5. Save the `.txt` file

#### On iPhone:
1. Open the WhatsApp chat you want to analyze
2. Tap the contact/group name at the top
3. Scroll down and tap **Export Chat**
4. Choose **Without Media**
5. Save the `.txt` file

### 2. Upload the Chat File

1. Open the Chat Analyzer application
2. Click on the file uploader
3. Select your exported `.txt` file
4. Wait for processing (you'll see a "Processing your chat..." animation)

### 3. Explore Your Results!

Once processing is complete, you'll see:

- **User Messages**: Raw parsed user messages with timestamps
- **System Messages**: System notifications from WhatsApp
- **Message Distribution Chart**: Bar chart showing messages per user
- **Top Contributor Badge**: Highlights the most active user
- **Most Used Words**: Displays frequently used words with usage count
- **Timeline Graph**: Line chart showing message activity over time

---

## 📊 What You'll Get

### 1. User Message Parsing
The analyzer extracts:
- Date and time of each message
- Sender's name
- Message content

### 2. Visual Analytics

#### Messages Per User
A horizontal bar chart showing how many messages each participant has sent, color-coded for easy identification.

#### Most Interactive User
A highlighted badge showing:
- Username of the top contributor
- Total messages sent
- Special "🔥 Top Contributor" indicator

#### Most Used Words
- Filters out common words (like "the", "and", "is")
- Ignores media omitted messages
- Shows words used most frequently
- Displays usage count

#### Timeline Analysis
- Hour-by-hour message distribution
- Interactive line chart
- Helps identify peak conversation times

---

## 🔧 Technical Details

### File Format Support
- **Supported**: `.txt` files (WhatsApp chat exports)
- **Date Format**: `DD/MM/YYYY HH:MM AM/PM`

### Filtering Intelligence
The analyzer automatically:
- Removes common stop words (a, the, is, are, etc.)
- Filters out media placeholder messages
- Handles multi-line messages correctly
- Distinguishes between user and system messages

### Technology Stack
- **Frontend**: Streamlit
- **Data Visualization**: Plotly Express
- **Language**: Python 3.x
- **Key Libraries**:
  - `streamlit` - Web interface
  - `plotly` - Interactive charts
  - `datetime` - Time parsing
  - `string` - Text processing

---

## 👥 Contributors

This project was collaboratively developed by a team of 3 developers.

---

## 📝 License

This project is open source and available for educational purposes.

---

## 🐛 Troubleshooting

### Issue: "Timeline could not be generated"
**Solution**: This happens when the date format in your chat doesn't match `DD/MM/YYYY HH:MM AM/PM`. Try exporting your chat again or check if the format is different.

### Issue: No messages showing
**Solution**: Ensure you exported the chat as a `.txt` file without media. Re-export and try again.

### Issue: Installation errors
**Solution**: Make sure you have Python 3.7+ installed. Try upgrading pip:
```bash
pip install --upgrade pip
pip install streamlit plotly
```

---

## 💡 Tips for Best Results

1. **Use group chats** for more interesting statistics
2. **Longer chat histories** provide better insights
3. **Export without media** for faster processing
4. **Try different chats** to compare activity patterns

---

## 📧 Support

If you encounter any issues or have suggestions, please create an issue in the repository or contact the development team.

---

**Made with ❤️ for WhatsApp users who love data!**
