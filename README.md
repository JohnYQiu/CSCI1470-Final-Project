Hello Professor Balestriero and CSCI1470 TAs!

Requirements:
torch>=2.0.0
pandas>=2.0.0
numpy>=1.24.0
scikit-learn>=1.3.0
matplotlib>=3.7.0

Overview: The COVID-19 pandemic sharply increased EMS call volume and strained dispatch centers worldwide. Workforce shortages, crowding, and process inefficiencies all factored into this situation. With several BEMS staff on our team, we sought to alleviate the bottleneck of EMS calls in similar high-demand situations, streamlining patient-to-care timelines and implementing rapid assessment through the assistance of Deep Learning. Our main goal was to build a model that would predict and determine transportation or refusal when encountering a patient in an EMS context. EMS request volume and time per request remain elevated post-pandemic. In any emergency medical context, we must be able to offer fast and accurate decision-making to maximize patient care if such a scenario were to arise. 

Files:
| ‘data/modified_fhir’ | 	FHIR JSON files manually edited from Synthea generated patients. We added extra labels (transport/non_transport) for our model.
| ‘fhir_parser.py’ | 		Parse all data into one tabular row for each EMS encounter
| ‘preprocessing.py’ | 		Preprocesses raw columns into model-ready features
| ‘models.py’ | 			Contains the main model and several other ML/DL models
| ‘train.py’ | 			Handles learning process (optimization, early stopping point)
| ‘eval.py’ | 			Evaluates model accuracy and performance
| ‘experiments.py’ | 		Runs analyses on inputs, alternative models, checks for completeness/robustness
| ‘main.py’ | 			Runs model/full workflow from data on computer
| ‘compare_models.py’ |	Compares various ML and DL models
| ‘requirements.txt’ | 		Requirements to run model

How to Run:
python main.py