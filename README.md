# Wildlife-Behavior-Prediction-using-Hidden-Markov-Model-HMM-

This project focuses on predicting wildlife behavior using Hidden Markov Models (HMM) applied to GPS tracking data. The goal is to identify distinct behavioral states from movement patterns and analyze their transitions.

# Key Features

1. Data Ingestion and Preprocessing: Handles diverse GPS tracking datasets from various animal species (e.g., lesser black-backed gulls, African buffalo, white storks).
2. Feature Engineering: Extracts meaningful features from raw GPS data, including 'hour', 'day_of_week', 'distance', and 'speed_diff', to enrich the dataset for behavioral analysis.
3. Hidden Markov Model (HMM) Implementation: Utilizes HMMs to model and predict latent behavioral states based on observed movement patterns.
4. Behavioral Analysis: Quantifies the duration spent in each predicted behavioral state and analyzes the transitions between these states using a behavior transition matrix.
5. Interactive Visualizations: Generates interactive maps and heatmaps to visualize animal movement and identified behavioral patterns.
   
# Project Structure

1. wildlife.ipynb: The main Jupyter Notebook containing all the code for data loading, preprocessing, feature engineering, HMM model training, and analysis.
2. lesser_black_backed_gulls_map.html: An interactive map visualizing the movement tracks of lesser black-backed gulls.
3. movement_heatmap.html: An interactive heatmap illustrating the density of animal movement.
4. hmm_model.pkl: The trained Hidden Markov Model, saved for future use and deployment.
5. dataset/:  Contains the raw GPS tracking data files used for the analysis.
   
# Methodology
6. Data Loading: GPS tracking data from various sources are loaded and merged into a single DataFrame.
7. Data Cleaning: Timestamps are converted, and missing values are handled through techniques like forward-filling.
8. Feature Creation: New features crucial for behavioral understanding, such as hourly and daily patterns, inter-point distance, and speed difference, are calculated.
9. HMM Training: A Hidden Markov Model is trained on the processed data to uncover hidden behavioral states (e.g., resting, foraging, traveling).
10. Behavior Prediction: The trained HMM is used to predict the most likely behavioral state for each recorded GPS point.
11. Visualization and Interpretation: Interactive maps and heatmaps are generated to provide visual insights into animal movements and behavioral transitions.
    
# Results
1. Identified Behavioral States: The HMM successfully identifies distinct behavioral states from the animal movement data.
2. Behavioral Duration Analysis: Visualizations show the total duration animals spend in each predicted behavior.
3. Transition Probabilities: A behavior transition matrix provides insights into the likelihood of moving from one behavioral state to another.
4. Movement Maps: Interactive maps visualize the precise GPS tracks, helping to understand spatial patterns of movement.
5. Movement Heatmaps: Heatmaps provide a density view of animal presence, highlighting high-activity areas.
