Recommendation System Project

Introduction


This project implements a recommendation system using three different models. Each model is designed to recommend items to users based on their preferences and past interactions.

Models

Model 1: Restricted Boltzmann Machine (RBM)

Description

The Restricted Boltzman model is used to predict recommendations based on user ratings. It works by modeling the user-item interactions and learning the underlying patterns in the data.

Training

The RBM is trained using the following steps:

Initialize the visible and hidden layers.
Perform Gibbs sampling to update the states of the visible and hidden units.
Calculate the reconstruction error and update the weights accordingly.
Usage
To use the RBM model for recommendations:

Train the model on the training dataset.
Use the trained model to predict recommendations for a given user.


Features
- Personalized Recommendations: Suggests movies based on user preferences.
- Scalability: Efficient for large datasets.
- Collaborative Filtering: Utilizes RBM for enhanced recommendations.


Model 2: Neural Collaborative Filtering (NCF)

Description

The NCF model uses neural networks to learn the user-item interactions. It combines the Generalized Matrix Factorization (GMF) and Multi-Layer Perceptron (MLP) techniques to provide accurate recommendations.


Training
The NCF model is trained by:


Initializing the user and item embeddings.
Passing the embeddings through multiple layers of neural networks.
Optimizing the model using a loss function such as Mean Squared Error (MSE).

Usage

To use the NCF model for recommendations:

Train the model on the training dataset.
Use the trained model to predict recommendations for a given user.


Model 3: Hybrid Model

Description

The Hybrid model combines the strengths of both RBM and NCF models to provide more accurate recommendations. It leverages the learned representations from both models to improve the prediction accuracy.

Training

The Hybrid model is trained by:

Training both RBM and NCF models separately on the training dataset.
Combining the outputs from both models to generate final recommendations.
Usage

To use the Hybrid model for recommendations:

Train both RBM and NCF models on the training dataset.
Use the trained models to predict recommendations for a given user.
Combine the recommendations from both models to get the final list.

Prerequisites
- Python 3.x
- PyTorch
- NumPy
- Pandas

Installation
1. Clone the repository:
   git clone <repository_url>
   cd <repository_directory>
2. Install the required packages:
   pip install -r requirements.txt

Usage
1. Prepare your dataset: Ensure your dataset is in CSV format with columns: userID, movieID, and rating.
2. Modify the script to point to your dataset file:
   df = pd.read_csv('path_to_your_dataset.csv')
3. Run the script:
   python movie_recommendation.py


Model Details
- Restricted Boltzmann Machine (RBM): A neural network used for collaborative filtering in recommendation systems, consisting of visible and hidden layers.

Contributing
Feel free to submit issues or pull requests. For major changes, please open an issue first to discuss the changes you wish to make.

License
This project is licensed under the MIT License - see the LICENSE file for details.
