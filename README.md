# MoodMuseModel
MoodMuse" – An AI-Powered Emotion-to-Art Generator


Project Overview

MoodMuse is an AI-powered tool that categorizes human moods from photographs using recognition of images and natural language processing. This research, which is housed on Hugging Face Spaces and was constructed using OpenAI's CLIP (Contrasting Language–Image Initial training) model, shows how multimodal artificial intelligence can decipher visual inputs (pictures) and link them to abstract human emotions. By analyzing facial expressions, settings, and tones to deduce emotions, MoodMuse seeks to investigate how AI may facilitate artistic, therapeutic, or recreational endeavours.

Tools and Technologies 

Hugging Face's Transformers library provided access to the openai/clip-vit-base-patch32 basic model, which forms the basis of this application. CLIP is a great option for image-to-text matching applications like mood categorisation since it can acquire visual concepts under natural language supervision. CLIPProcessor is used to process the incoming image, encoding it along with a list of potential mood labels. To determine which mood is most comparable, the generated image and text embeddings are compared.
A simple and interactive web interface was created using Gradio, enabling users to upload photos and get mood forecasts in real time. The Hugging Face authentication token (HUGGINGFACEHUB_API_TOKEN), which is controlled by environment variables for security, provides secure access to the model when the app goes live on Hugging Face Spaces.

How It Works

The Gradio interface is used by users to upload images. A predetermined set of emotions, including "happy," "sad," "anxious," and "hopeful," is then associated with the image. CLIP contrasts each mood's textual representation with its graphic counterpart. After calculating similarity scores, it provides a confidence percentage and the emotional label with the greatest score.
How to Run It
Install dependencies using pip install -r requirements.txt and set the environment variable HUGGINGFACEHUB_API_TOKEN with your own Hugging Face token to launch the project locally. Next, use Python moodmuse.py to launch the application. Set your token under the Secrets page under Advanced Settings and upload your code and materials for Hugging Face Spaces deployment.


