# AI Auto Repair Visual Assistant

## Overview

AI Auto Repair Visual Assistant is a multimodal AI tool designed for an emerging auto repair shop. It accepts a vehicle image and a text question and uses a vision-language AI model to provide visual observations, possible inspection areas, and recommended next steps.

The tool is intended for preliminary inspection support and does not replace a professional mechanic's diagnosis.

## Scope

The tool focuses on analyzing vehicle images together with user questions. It can help identify visible vehicle conditions and suggest areas that may need further inspection.

## Features

* Accepts vehicle images
* Accepts text questions
* Uses multimodal AI for image and text analysis
* Provides visual observations
* Suggests possible inspection areas
* Recommends next steps
* Handles missing image errors
* Tests unusual user questions

## Tools and Technologies

* Python
* Jupyter Notebook
* Hugging Face Inference API
* Qwen2.5-VL-72B-Instruct
* Base64 image encoding

## How It Works

1. The user provides a vehicle image.
2. The user enters a question about the image.
3. The image is encoded and sent with the question to the AI model.
4. The AI analyzes both inputs.
5. The tool displays the vehicle image and AI response.

## Testing

The tool was tested using three vehicle images.

Additional tests were performed for:

* Missing image input
* Empty question input
* Unusual request for exact repair cost

The missing image test produced an error message instead of stopping the notebook. The empty question was accepted by the model and still produced an image analysis. The exact repair cost test showed that the AI could not determine an exact cost from an image alone and recommended professional inspection.

## Problems and Fixes

During development, different AI model configurations were tested. Some models were unavailable or had capacity limitations. The final working configuration uses Qwen2.5-VL-72B-Instruct through Hugging Face Inference Providers.

An OpenAI API approach was also tested but could not be used because the available API account had no usable credit balance.

## Professional Examples Researched

### 1. PakWheels

PakWheels provides professional car inspection services in Pakistan. Its inspection covers 200+ checkpoints, including the engine, suspension, exterior, interior, electrical systems, and safety-related areas. It also provides a digital inspection report.

### 2. AutoFirst

AutoFirst provides a platform for generating professional car inspection reports. It helps users understand a vehicle's condition, price, and possible repairs. It also offers plans for individual and business users.

### 3. CarOK

CarOK provides vehicle inspection services in Pakistan. Its inspection includes mechanical, body, electrical, and other vehicle checks, followed by a scored digital report. CarOK also provides AI-based tools, including photo inspection and an AI risk score.

### Relevance to This Project

These Pakistani examples show how vehicle inspection and AI-based automotive tools can support vehicle assessment. This project uses a simpler multimodal approach by combining a vehicle image with a text question to provide preliminary observations and recommended inspection areas.


## Limitations

The tool only analyzes information visible in the provided image and the user's question. It cannot confirm internal mechanical problems or provide an exact repair cost. A professional mechanic should perform the final inspection and diagnosis.

## Future Improvement

With more development time, the tool could include a simple user interface where a repair shop employee can upload an image and enter a question without editing the notebook code.

## Project Files

* `AI_Auto_Repair_Visual_Assistant.ipynb` – Main project notebook
* `requirements.txt` – Required Python package
* `PROJECT_SUMMARY.md` – Project summary
* `images/` – Vehicle test images
* `screenshots/` – Project evidence screenshots
