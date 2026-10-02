Prompt-Based Virtual Try-On Using Stable Diffusion & ControlNet

This project is a Generative AI-based Prompt-Based Virtual Try-On system that generates realistic fashion images by combining a person’s photograph with a text-based clothing description. The system uses **Stable Diffusion 1.5, ControlNet, and OpenPose to control the generation process and maintain the person’s body pose.

The workflow starts with a user-provided image, which is processed using OpenPose to detect the human body structure and generate a pose representation. This pose information is provided to ControlNet, allowing the diffusion model to preserve the spatial and structural characteristics of the original person while generating a new appearance.

A text prompt describes the desired clothing and visual style, such as a specific dress, color, or fashion appearance. Stable Diffusion uses this textual information together with the ControlNet pose conditioning to generate the final image. Positive prompts guide the desired appearance, while negative prompts help reduce unwanted characteristics such as blurry images, poor quality, distorted bodies, and incorrect anatomy.

The implementation is developed in Python using PyTorch, Hugging Face Diffusers, OpenCV, and Pillow. GPU acceleration is used to improve the performance of the diffusion-based image generation process.

The project demonstrates the practical application of Generative AI, Diffusion Models, Computer Vision, Pose Estimation, and Controlled Image Generation in the fashion domain. It can serve as a foundation for more advanced virtual try-on systems that incorporate actual garment images, segmentation, garment masking, and improved identity preservation.
