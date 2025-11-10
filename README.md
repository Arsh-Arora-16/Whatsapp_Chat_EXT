# 📱 WhatsApp Real Estate Chat Extractor  
**Automated pipeline to filter, structure, and classify real-estate listings from WhatsApp group chats.**

This project processes WhatsApp group exports and converts messy property messages into clean, structured Excel sheets — categorized by property size, location, type, demand, and more.  
It is built for brokers operating in Mohali/Tricity who handle dozens of property groups and need accurate, searchable data.

---

## 🚀 Features

### 🏡 **Real Estate–Focused Parsing**
- Extracts property listings from WhatsApp messages  
- Detects sizes: *marla, gaj/yd, sq.ft, sq.yd, kanal*  
- Extracts contact numbers, addresses, sectors, floors, road type, direction  
- Removes rent listings by default  
- Handles groups with lots of noise (media omitted, emojis, all caps text)

### 🔍 **Smart Message Filtering**
- Only keeps messages with contact numbers  
- Removes system messages (joined, encryption, etc.)  
- Deduplicates listings across multiple groups  
- Includes only messages from **2025 onwards**

### 📊 **Clean Structured Output**
Creates:
- `structured_cleaned_chat.xlsx`  
- Classified sheets inside `classified_output/`  
- Final cleaned classification in `final_classified_output/`  
- A text file of unique filtered messages

### 📂 **Multi–Group Compilation**
If you have 50–100 groups:
- Place each exported folder → project directory  
- Script compiles all `_chat.txt` files  
- Automatically extracts real-estate listings  
- Outputs one master dataset

---

## 📁 Folder Structure

