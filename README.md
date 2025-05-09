# MoodMuseModel
MoodMuse" – An AI-Powered Emotion-to-Art Generator


# 🎵 MoodMuse: Emotion-Based Music Recommender

MoodMuse is a fun, AI-powered app that detects your facial emotion and recommends music to match your mood. Just upload a photo and get a playlist that resonates with how you're feeling!

-------------------------------------------------------------------------------------------------------------------------

## ✅ What the Project Does

- Detects emotion from a user's face using a pre-trained vision model.
- Maps the detected emotion (e.g., happy, sad, angry) to a curated list of songs.
- Recommends mood-matching music instantly via an interactive web interface.

--------------------------------------------------------------------------------------------------------------------------

## 🛠 Tools, Models, and APIs Used

| Tool / Library      | Purpose                                           |
|---------------------|---------------------------------------------------|
| `gradio`            | User interface and image upload frontend          |
| `transformers`      | Access to Hugging Face models                     |
| `CLIP (openai/clip-vit-base-patch32)` | Used to embed images and classify emotions |
| `torch`, `PIL`      | Image preprocessing and tensor handling           |
| `Python 3.8+`       | Backend development                               |

-------------------------------------------------------------------------------------------------------------------------

## 🚀 How to Run It Locally

1. **Clone this repo**:
   ```bash
   git clone https://huggingface.co/spaces/jyotipriya/moodmuse
   cd moodmuse


