# Amazon Music Clustering & Analysis

This project focuses on analyzing and clustering Amazon Music data using Machine Learning techniques. The goal is to identify patterns, group similar items, and extract meaningful insights from the dataset.

## Project Overview
🔍 Perform data preprocessing and cleaning
📊 Apply clustering algorithms to group similar data
📈 Visualize clusters for better understanding
🧠 Analyze patterns and insights from grouped data

## Features
Data cleaning and preprocessing
Feature engineering
Clustering using algorithms like:
K-Means
Hierarchical Clustering (if used)
Visualization using:
Matplotlib
Seaborn
Cluster interpretation and analysis

## Project Structure
📁 amazon-music-clustering
│
├── 📄 amazon_music_clustering.ipynb   # Main notebook
├── 📄 README.md                      # Project documentation
├── 📁 data                           # Dataset (if included)
└── 📁 outputs                        # Results & visualizations

## Installation
Clone the repository:
git clone https://github.com/your-username/amazon-music-clustering.git
cd amazon-music-clustering
Install dependencies:
pip install -r requirements.txt
▶️ Usage

Run the Jupyter Notebook:

jupyter notebook amazon_music_clustering.ipynb

Or open it in Google Colab.

## Workflow
Load dataset
Clean & preprocess data
Feature scaling
Apply clustering algorithm
Evaluate clusters
Visualize results

## Sample Outputs
Cluster plots
Elbow method graph
Cluster distribution

## Insights
Identified groups of similar music patterns
Found trends in user preferences / audio features
Improved understanding of dataset structure

## Technologies Used
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib
- Streamlit

##  Machine Learning Approach

### 1. Data Preprocessing
- Removed duplicates
- Selected numeric features
- Handled missing values
- Standardized features using `StandardScaler`

---

### 2. Optimal Clusters Selection
- Used **Silhouette Score**
- Tested values of k (2–5)
- Selected best k based on highest score

---

### 3. Clustering
- Applied **KMeans Clustering**
- Assigned cluster labels:


---

### 4. Mood Classification
Clusters are mapped to moods using feature thresholds:

| Condition | Mood |
|----------|------|
| High energy + high valence | Happy / Energetic |
| High acousticness | Calm / Acoustic |
| Low energy | Sad / Chill |

---

### 5. Visualization
- PCA used to reduce dimensions to 2D
- Scatter plot shows clusters

---

## Output
- `outputs/clustered_songs.csv`
- Contains:
- Features
- Cluster labels
- Mood labels

---

##  Streamlit Dashboard
Features:
- Filter by cluster
- View songs per cluster
- Visualize feature relationships
- Display statistics

Run locally:
```bash
streamlit run app.py
  
## License

This project is open-source and available under the MIT License.

👤 Author

Muthu
Scikit-learn
Matplotlib / Seaborn
Jupyter Notebook
