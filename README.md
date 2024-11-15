# AI-Powered-Personalized-Floor-Plans-Innovative-Architectural-Design

*Problem Statement:*
Developing a system that generates personalized architectural layouts based on user descriptions of apartment features.

*Dataset Description:*
The dataset was taken from huggingface and is stored in parquet format.
This experimental dataset is designed for training conditional text-to-image models specifically for generating detailed architectural floor plans. Unlike basic wall and room segmentation, this dataset includes comprehensive controls such as walls, rooms, and footprint boundaries.

The dataset includes:

Indices- Unique identifiers for each architectural layout.
Plans - Image files representing detailed architectural floor plans.
Walls - Image files showing the locations and dimensions of walls.
Colors - Image files depicting the color schemes used in the layouts.
Footprints - Image files outlining the boundaries of structures within the plans.
Plan_captions - Text descriptions providing context for each floor plan.


The dataset is of parquet format which is a columnar storage format designed for efficient data compression and fast querying in big data processing.

*Algorithms Used:*
1. CGAN(Conditional Generative Adversarial Network)
   A type of Generative Adversarial Network tailored for image generation.

-Consists of a generator that creates images and a discriminator that evaluates their realism.

-In a CGAN, the generator is conditioned on specific text inputs (from BERT embeddings) to generate images that align with given descriptions.

2. BERT (Bidirectional Encoder Representations from Transformers):

A powerful NLP model used to transform text descriptions into vector embeddings.

These embeddings serve as the conditioning input to the CGAN, guiding the generator to produce images that match the textual prompts.

- Enhances the model’s ability to understand and generate images that are relevant to the provided descriptions. 


Visit the following google drive to access the files used for deployment of the project:
https://drive.google.com/file/d/17rUPng5fucA8d3r87BeStvqIzQ4pk4CO/view?usp=sharing

Visit the following google drive to look at the video demo of the project:
https://drive.google.com/file/d/1KVjjqPI0FVceKkEhjFuc4_l603CU2nHv/view?usp=sharing


*Future Works*:
Though the model is working fine with acceptable error metrics, the image being generated is not upto the mark and need more fine-tuning. Implementation of stable diffusion for this project will help achieving desirable results.





