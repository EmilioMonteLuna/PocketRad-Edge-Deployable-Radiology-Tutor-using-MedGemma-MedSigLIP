# PocketRad —  Radiology Education with MedGemma + MedSigLIP

Retrieval-augmented chest X-ray education tool using Google's HAI-DEF models.
Upload a CXR → retrieve 3 visually similar confirmed cases → get a grounded educational explanation.

## Setup (Required Before Running)

1. **HF_TOKEN** — Accept MedGemma terms at https://huggingface.co/google/medgemma-4b-it  
   Then get your token at https://huggingface.co/settings/tokens  
   Add as Colab Secret named: `HF_TOKEN`

2. **NGROK_TOKEN** — Sign up free at https://ngrok.com  
   Get token at https://dashboard.ngrok.com/get-started/your-authtoken  
   Add as Colab Secret named: `NGROK_TOKEN`

3. Open notebook in Colab → Runtime → Run All  
   Full setup: ~25 minutes

## Stack
- MedSigLIP (`google/medsiglip-448`) — visual retrieval
- MedGemma 4B (`unsloth/medgemma-4b-it-bnb-4bit`) — explanation generation  
- Streamlit — UI
- Indiana University CXR dataset — 7,470 chest X-rays

## Disclaimer
For educational use only. Not for clinical diagnosis.
