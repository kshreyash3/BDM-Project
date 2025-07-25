# BDM-Project

## Customer Behavior Analysis and Recommendation System for E-commerce

This project implements a scalable product recommendation system for an e-commerce platform. It utilizes user behavior data such as clicks, views, and purchases to generate real-time personalized product suggestions using collaborative and content-based filtering techniques.

## Technology Stack
- Data Ingestion: CSV 
- Data Storage:  Pandas
- Data Processing: PySpark / Pandas
- Modeling: ALS (Spark MLlib), TF-IDF (Scikit-learn)
- API Development: Flask
- Data Visualization: Matplotlib, Seaborn

## Dataset
The dataset contains user activity data including user IDs, product IDs, event types (view, click, purchase), timestamps, and product metadata.

## Modeling Approaches
- Collaborative Filtering: Utilizes the Alternating Least Squares (ALS) algorithm for implicit feedback.
- Content-Based Filtering: Applies TF-IDF vectorization on product descriptions and uses cosine similarity for recommendations.

## API Demonstration
- Endpoint: `GET /recommendations?user_id=<USER_ID>`
- Sample Response:
```json
{
  "user_id": "U123",
  "recommended_products": ["Product A", "Product B", "Product C"]
}
```

## How to Run
```bash
pip install -r requirements.txt
jupyter notebook BDM_Project.ipynb
python app.py  # Launches the Flask API server
```

## Future Enhancements
- Integration with real-time data streaming using Kafka
- Deployment on cloud platforms such as AWS or GCP
- Implementation of deep learning-based recommendation algorithms
