# Fitness Tracker with Real-Time Insights and Recommendations  

This project provides a pipeline to extract insights from a fitness tracker dataset, integrate real-time insights with a Recommendation-Augmented Generation (RAG) system, and visualize results using Streamlit.  

---

## Table of Contents  
1. [Features](#features)  
2. [Technologies Used](#technologies-used)  
3. [Project Structure](#project-structure)  
4. [Setup Instructions](#setup-instructions)  
5. [Acknowledgments](#acknowledgments)  

---

## Features  
- **Insight Extraction**: Real-time data processing using Pathway to derive key insights from the fitness tracker dataset.  
- **RAG Implementation**: Recommendations generated using Gemini LLM based on extracted insights.  
- **Visualization**: A Streamlit app to visualize the dataset with the added recommendations column.  

---

## Technologies Used  
- Python  
- Jupyter Notebook  
- Pathway for real-time data streaming and processing  
- Gemini LLM API for generating recommendations  
- Streamlit for visualization  

---

## Project Structure  
The repository is organized as follows:  
```plaintext  
├── notebooks/  
│   ├── 01_extract_insights.ipynb   # Extracting insights from the dataset  
│   ├── 02_perform_rag.ipynb        # Generating recommendations and saving results  
│   ├── 03_visualize_streamlit.ipynb  # Streamlit-based CSV visualization  
├── requirements.txt                # Python dependencies  
├── README.md                       # Project documentation  
├── small_dataset.csv                     # Example dataset used  
├──Database/                       # Database folder  
│   ├── fitness_tracker.db         # SQLite database  
```

---

## Setup Instructions  
1. Clone the repository:  
   ```bash  
   git clone https://github.com/Harsh-D-2004/Quarks_Hackathon.git
   ```
2. Setup the Python environment:  
    ```bash 
    python -m venv q_env  
    source q_env/bin/activate  
    pip install -r requirements.txt
    ```
3. Configure Environment Variables
    ```bash 
    GEMINI_API_KEY=your_gemini_api_key  
    ```
4. Run Jupyter Notebooks
    Navigate to the notebooks/ directory and execute the notebooks in sequence:

    Extract Insights: 01_extract_insights.ipynb
    Processes the dataset and streams live data using Pathway.

    Perform RAG: 02_perform_rag.ipynb
    Uses Pathway insights and passes them to Gemini LLM to generate recommendations, adding them as a new column in result.csv.

    Streamlit Visualization: 03_visualize_streamlit.ipynb
    Visualizes the results in result.csv using Streamlit.er notebook  

5. Run Streamlit App
    ```bash
    streamlit run notebooks/03_visualize_streamlit.ipynb  
    ```
---

## Acknowledgments
Pathway: For real-time insights extraction.
Gemini LLM API: For generating personalized recommendations.
Streamlit: For building the visualization dashboard.

---