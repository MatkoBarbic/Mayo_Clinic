# Mayo_Clinic - Image Classification of Stroke Blood Clot Origin

Link to the competition: "https://www.kaggle.com/competitions/mayo-clinic-strip-ai"

The goal of the competition is to classify two types of blood clots using whole slide digital pathology images.
The biggest problem in this competition was handling large images with the biggest being as big as 4.9 GB. This was done by using OpenSlide library and splitting the images into tiles. Since a lot of the images are mostly white space, I discarded tiles that are mostly or fully blank using the thresholding technique.

Using EfficientNet I managed to obtain a 72% accuracy which is a good result in my opinion.

Tiling notebook link: "https://www.kaggle.com/code/matkobarbic/dataset-tiling"
EfficientNet notebook link: "https://www.kaggle.com/code/matkobarbic/mayo-effnet"
