# Internship-at-mirai-assignment-4

## Multi-Modal Visual Novel
Capstone mini-project for the MirAI School of Technology Virtual Summer Internship 2026, AI Builder Track.

This project is a Streamlit-based "Choose Your Own Adventure" visual novel engine. It uses Gemini for stateful story generation, Pollinations for visual scene generation, Python JSON parsing for structured AI output, dynamic Streamlit buttons for player choices, and gTTS for browser-playable narration.



https://github.com/user-attachments/assets/8a746960-2463-41fd-8b13-03ef6bc61021

## Features
- Stateful visual novel flow using st.session_state
- Cached Gemini client using @st.cache_resource
- Sidebar story configuration for genre and art style
- Strict Gemini JSON response format:
 -- story_text
 -- image_prompt
 -- options
- JSON parsing with Python's built-in json library
- Dynamic choice buttons generated from Gemini's options list
- Pollinations image generation from the AI-produced image_prompt
- Text-to-speech narration with gTTS
- Streamlit audio playback with st.audio()
- Graceful failure handling with try...except and st.toast()
