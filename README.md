

# 🇧🇷 Brazilian Slang API

The **Brazilian Slang API** helps developers, students, and travelers discover real Portuguese expressions used in Brazil every day.

## 🌍 Base URL

http://189.126.106.151/

## 🧩 Endpoints

### 1️⃣ GET `/api/slang`
Returns a random Brazilian slang word with translation and example.

**Example Request:**
```bash
curl --request GET --url 'http://189.126.106.151/api/slang'

Example Response:

{ "word": "beleza", "translation": "cool / all good", "example": "Beleza, vamos! (Cool, let's go!)" }

2️⃣ GET /api/slang?word={word}

Returns details of a specific slang word.

Example Request:

curl --request GET --url 'http://189.126.106.151/api/slang?word=valeu'

Example Response:

{ "word": "valeu", "translation": "thanks / cool", "example": "Valeu pelo apoio! (Thanks for the support!)" }

⚠️ Error Example

{ "error": "Slang not found" }
