# Project Summary

## AI Auto Repair Visual Assistant

This project develops a multimodal AI tool for an emerging auto repair shop. The tool combines a vehicle image with a text question and uses a vision-language AI model to provide preliminary visual observations, possible inspection areas, and recommended next steps.

The project was developed using Python and Jupyter Notebook with the Hugging Face Inference API and Qwen2.5-VL-72B-Instruct model.

The tool was tested with three vehicle images and different types of user input. Testing also included a missing image, an empty question, and an unusual request for an exact repair cost. These tests showed that the tool can analyze vehicle images successfully, handle missing image errors, and recognize limitations when information is not available from an image alone.

During development, several model configurations were tested before selecting a working model through Hugging Face Inference Providers. The final tool provides useful preliminary inspection support but does not replace a professional mechanic's diagnosis.

With more development time, a simple user interface could be added so repair shop employees can upload an image and enter questions without editing notebook code.
