# <center><b>Recommendation System Project</b></center>

This project implements a recommendation system using three different models. Each model is designed to recommend items to users based on their preferences and past interactions.

---

## <b>Models</b>

### <b>Model 1: Restricted Boltzmann Machine (RBM)</b>

#### <b>Description</b>
The Restricted Boltzmann Machine (RBM) is used to predict recommendations based on user ratings. It works by modeling the user-item interactions and learning the underlying patterns in the data.

#### <b>Training</b>
The RBM is trained using the following steps:
1. Initialize the visible and hidden layers.
2. Perform Gibbs sampling to update the states of the visible and hidden units.
3. Calculate the reconstruction error and update the weights accordingly.

#### <b>Usage</b>
To use the RBM model for recommendations:
1. Train the model on the training dataset.
2. Use the trained model to predict recommendations for a given user.

#### <b>Features</b>
- Personalized Recommendations: Suggests items based on user preferences.
- Scalability: Efficient for large datasets.
- Collaborative Filtering: Utilizes RBM for enhanced recommendations.

---

### <b>Model 2: Neural Collaborative Filtering (NCF)</b>

#### <b>Description</b>
The NCF model uses neural networks to learn the user-item interactions. It combines the Generalized Matrix Factorization (GMF) and Multi-Layer Perceptron (MLP) techniques to provide accurate recommendations.

#### <b>Training</b>
The NCF model is trained by:
1. Initializing the user and item embeddings.
2. Passing the embeddings through multiple layers of neural networks.
3. Optimizing the model using a loss function such as Mean Squared Error (MSE).

#### <b>Usage</b>
To use the NCF model for recommendations:
1. Train the model on the training dataset.
2. Use the trained model to predict recommendations for a given user.

---

### <b>Model 3: Hybrid Model</b>

#### <b>Description</b>
The Hybrid model combines the strengths of both RBM and NCF models to provide more accurate recommendations. It leverages the learned representations from both models to improve the prediction accuracy.

#### <b>Training</b>
The Hybrid model is trained by:
1. Training both RBM and NCF models separately on the training dataset.
2. Combining the outputs from both models to generate final recommendations.

#### <b>Usage</b>
To use the Hybrid model for recommendations:
1. Train both RBM and NCF models on the training dataset.
2. Use the trained models to predict recommendations for a given user.
3. Combine the recommendations from both models to get the final list.

---

## <b>Prerequisites</b>
- Python 3.x
- PyTorch
- NumPy
- Pandas

---

## <b>Installation</b>
1. Clone the repository:
   git clone <repository_url>
   cd <repository_directory>
2. Install the required packages:
   pip install -r requirements.txt

---

<b>Usage</b>
1. Prepare your dataset: Ensure your dataset is in CSV format with columns: userID, movieID, and rating.
2. Modify the script to point to your dataset file:
   df = pd.read_csv('path_to_your_dataset.csv')
3. Run the script:
   python movie_recommendation.py

---

<b>Model Details</b>
Restricted Boltzmann Machine (RBM): A neural network used for collaborative filtering in recommendation systems, consisting of visible and hidden layers.
<b>Contributing</b>
Feel free to submit issues or pull requests. For major changes, please open an issue first to discuss the changes you wish to make.

<b>License</b>
This project is licensed under the MIT License - see the LICENSE file for details.
