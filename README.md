# Cooking Buddy 🍳  

I built this project to solve one of the most common daily struggles I face — figuring out what to cook with whatever ingredients I have in my kitchen.
Cooking Buddy is a friendly AI assistant that helps you decide what to make based on your available ingredients and dietary needs. You can either type or speak your input naturally (just like talking to a friend!), and the bot will suggest fun, creative meals tailored to what you have — no fancy stuff, just what's in your pantry and fridge. You can even get a dish image and save everything as a PDF for later.

## Models Used  
- **GPT-4o-mini (x4)**: Used in a multi-step pipeline:
  1. Extract structured ingredients and diet preferences from casual speech/text  
  2. Suggest creative recipe ideas based on available ingredients and common pantry items 
  3. Filter recipes by dietary rules (e.g. allergies, kosher, vegan)  
  4. Generate full, friendly, step-by-step recipes with emojis, tips, and substitutions

- **Whisper (speech-to-text)**: Converts audio input into natural text for both ingredients and dietary info.

- **DALL·E-2**: Optionally generates an image preview of the first suggested dish.

## Features  
- Supports **voice or text input** for both ingredients and preferences  
- Generates **personalized, creative recipes** based on available items  
- Filters recipes to **respect dietary rules** (e.g., allergies, kosher, vegan)  
- Produces **a visual dish preview** using generative image models  
- Allows **PDF export** of recipes for offline use

## How It Looks

**Start Screen**  
<div align="center">  
<img src="https://github.com/user-attachments/assets/b0554b6e-94cd-49bb-b5c9-268341affd5a" width="600"/>
</div>

**Voice Input with Option to Reset Recording**  
<div align="center">  
<img src="https://github.com/user-attachments/assets/c5bff7f4-88f7-453e-9be5-831c0c940389" width="600"/>
</div>

**AI-Generated Image for Top Dish & Start of Response**  
<div align="center">  
<img src="https://github.com/user-attachments/assets/3f7fb6c4-6848-4629-9d60-e16ebe5c4728" width="600"/>
</div>

**Generated Full Recipes with Instructions and Tips**  
<div align="center">  
<img src="https://github.com/user-attachments/assets/be024614-deeb-4885-8d2e-ab4c0403295e" width="600"/>
</div>

**Option to Export All Recipes as PDF**  
<div align="center">  
<img src="https://github.com/user-attachments/assets/d47943c7-4ad6-4b81-b2bb-5f2eaf07a4af" width="600"/>
</div>

## What I learned:
This was a self-initiated learning project, driven by curiosity and a desire to explore GenAI in practice. I researched and experimented with every part of the stack independently, diving deep into each model's capabilities and limitations. I learned how to move from idea to working prototype, building a real solution to a real problem in my daily life.
- Designed a multi-stage pipeline using LLMs for natural input cleaning, idea generation, filtering, formatting, and for a seamless multi-modal UX
- Handled natural language input variability, user intent, and dietary logic
- Built an interactive, app-like user experience with Streamlit


## 🔧 Installation & Setup
Install the required packages with:
```bash
pip install -r requirements.txt
```
Make sure to add your OpenAI API key in a .env file like this:
```bash
OPENAI_API_KEY=your_key_here
```
then run:
```bash
streamlit run bot.py
```

👥 This project was created by Shira Aronovich.
