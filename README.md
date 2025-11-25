🌿 Medicinal Plant Classification using Simple CNN

A deep learning–based capstone project for identifying 20 medicinal plant species from leaf images using a custom Convolutional Neural Network (CNN) model.

📌 Project Overview

This project focuses on building a Simple CNN model to classify medicinal plants using leaf images.
The model is trained on a Kaggle dataset consisting of 20 plant classes.
Users can either upload their own leaf image or select a random image from the dataset to get predictions.

The system also returns medicinal benefits of each identified plant using a built-in knowledge base.

🌱 Features

✔️ Classifies 20 medicinal plant species
✔️ Simple custom CNN (no transfer learning)
✔️ Upload image or use random dataset sample
✔️ Displays the selected image
✔️ Provides medicinal uses of each plant
✔️ Logs classification history in memory
✔️ Interactive UI using Jupyter widgets

🗂️ Dataset Used(Primary Dataset)

Kaggle Dataset: Medicinal Leaf Augmented Dataset(Collected By Me )
Contains 20 classes, each with multiple augmented images. Classes included:

Akondo, Ashok, Basil, Cannonball_Tree, Cordia, Debdaru, Ginger,
Holud_pata, Jarul, Mastwood, Minjiri, Nageshor, Neem,
Pathorkuchi, Punnag, Royna, Tejpata, Telakucha, Thankuni, Vasaka
<img width="452" height="781" alt="image" src="https://github.com/user-attachments/assets/db8f9bf2-04a4-42a6-a522-b980000cb1dc" />

🧠 Model Architecture (Simple CNN)

Your model uses a lightweight CNN with layers such as:

Conv2D

MaxPooling2D

Dropout

Flatten

Dense layers

Output layer uses softmax for 20-class classification.
Conv2D → ReLU  
MaxPool  
Conv2D → ReLU  
MaxPool  
Flatten  
Dense (128)  
Dense (20 softmax)

🛠️ Tech Stack
Component	Technology
Model	Simple CNN (Keras / TensorFlow)
Interface	Jupyter Notebook + ipywidgets
Images	PIL
Memory Logging	Custom Python Class
Dataset	Kaggle

📥 How to Run
1️⃣ Install dependencies
pip install tensorflow pillow ipywidgets

2️⃣ Load the dataset in Kaggle Notebook

Place the dataset in:

/kaggle/input/medicinal-leaves-for-hybridvit-and-vgg19/

3️⃣ Run model training
model.fit(train_data, validation_data=val_data, epochs=20)

4️⃣ Save the model
model.save("medicinal_plant_classifier.keras")

5️⃣ Use the interactive UI to classify images

You can upload an image or let the system pick a random one.

🧾 Medicinal Knowledge Base

The system automatically returns medicinal information for each plant:

Example:

"Neem": "Neem leaves have antibacterial, antifungal, and antiviral properties and are used for skin and blood purification."


The full plant_info_db is embedded in the project as a Python dictionary.

📈 Accuracy

The Simple CNN achieves around 83.28% on validation data.

🎯 Use Cases

Herbal research

Agriculture

Educational projects

Real-time medicinal plant identification

Botanical assistance systems

📜 License

This project is for educational and research purposes.

CLASSES:
<img width="1123" height="587" alt="image" src="https://github.com/user-attachments/assets/f1c3371c-50e2-4f3d-830c-bb6d76d5bfbe" />
MODEL DESCRIPTION:
<img width="787" height="503" alt="image" src="https://github.com/user-attachments/assets/6d9017c3-2bcf-4708-bf2d-39534da7f062" />
EPOCHS:
<img width="1143" height="648" alt="image" src="https://github.com/user-attachments/assets/5f7b48c9-0f5a-419b-9498-b070298e1f06" />
OUTPUT :
<img width="642" height="527" alt="image" src="https://github.com/user-attachments/assets/441fbd4c-b2ba-48b8-afb8-ce429964676d" />
<img width="1142" height="362" alt="image" src="https://github.com/user-attachments/assets/69990f76-d094-4884-a7c3-74f13dc0afb9" />
<img width="1283" height="608" alt="image" src="https://github.com/user-attachments/assets/fca4b45d-1bb4-4154-8547-394bfe037750" />





