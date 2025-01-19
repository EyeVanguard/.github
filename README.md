# Eye Vanguard

The EyeVanguard project combines ophthalmological knowledge with technology to offer a complete solution for medical practitioners. A thorough explanation of the implementation procedure may be found below.

## Problem
Progressive damage to the optic nerve is the cause of glaucoma, one of the major causes of irreversible blindness in the world. More than 80 million people worldwide are impacted by it, and as the population ages, its prevalence is expected to increase. Early identification is essential to preventing visual loss because the disease advances silently and doesn't exhibit any symptoms until it is advanced. Despite their effectiveness, current diagnostic methods—such as visual field testing, intraocular pressure monitoring, and optic nerve imaging—are sometimes hindered by subjectivity, time constraints, and the availability of specialized ophthalmologists, especially in settings with limited resources.

The emergence of automated detection systems driven by machine learning and image processing offers a revolutionary way to tackle these issues.


## Features
- Fundus Image Analysis: glaucoma detection through AI-powered analysis of retinal fundus images.
- Research Hub: A well-selected database of the most recent ophthalmology research publications. Compatibility with hospital systems for effective data sharing is known as "smooth integration."

## Components
- [Frontend](https://github.com/EyeVanguard/Frontend): Frontend WebApp built using ReactJs to enable easy interaction with the ML model.
- [Backend](https://github.com/EyeVanguard/Backend): NodeJS Backend built using AdonisJS to seemlessly connect frontend to the ML model via powerful REST Apis
- [Machine Learning Model](https://github.com/EyeVanguard/ModelDevelopment): Models that can identify glaucoma by examining fundus images.

## Workflow

#### Segmentation and preprocessing
Preprocessing is done on retinal fundus pictures to improve quality and eliminate noise. To compute important metrics like the cup-to-disc ratio, the optic nerve head is segmented.
Using sophisticated image processing techniques, features are extracted, and machine learning models that have already been trained are used to analyze them.
The models are tested against test datasets that have not yet been seen after being trained on publicly accessible datasets (such as RIGA and Drishti-GS).

#### Backend and API Development
AdonisJS manages API requests for the analysis, retrieval of processed results, and uploading of images.
The backend's incorporation of machine learning models guarantees smooth fundus picture analysis.

#### Frontend Development
The user interface's easy navigation, image upload, and result display are powered by React.js. To give real-time feedback, the frontend uses RESTful APIs to communicate with the backend.



  
