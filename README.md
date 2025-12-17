# Fine-tuned-Bias-Detection-and-Counter-Argument-Generation-model  

This repository implements **a two-stage NLP pipeline**:  

1. Bias Detection: A fine-tuned BERT model (>98% accuracy) classifies news articles as _left, center, or right_.
2. Counter-Argument Generation: A fine-tuned FLAN-T5 model generates a coherent counter-argument from the opposite political stance.  

**Setup**
Clone the repository:

  git clone https://github.com/Sandesh816/Fine-tuned-Bias-Detection-and-Counter-Argument-Generation-model.git  
  cd Fine-tuned-Bias-Detection-and-Counter-Argument-Generation-model  

**Running the Project**

Open the main notebook directly in Colab (Recommended):  
	•	Model_training_and_finetuning.ipynb
  
Make sure to:  

•	Make a copy of the project: File → Save a copy in Drive  
•	Enable GPU: Runtime → Change runtime type → GPU (A100 preferred)  
•	(Optional) Add your Hugging Face token as a Colab secret (HF_TOKEN) for faster model downloads  
  
The notebook is organized into:  

•	Phase 1: Dataset loading, preprocessing, bias classification, rationale extraction  
•	Phase 2: Prompt construction, teacher (FLAN-T5-XL) generation, student fine-tuning, evaluation  
 
**Data**
The project automatically downloads the AllSides/QBias dataset from GitHub during execution.  
No manual data download is required.

**Outputs**  
	•	Trained bias classifier   
	•	Generated rationales  
	•	Counter-arguments from the opposite stance  
	•	Evaluation metrics (accuracy, confusion matrices, flip-rate)  






