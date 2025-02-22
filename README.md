# HybridFlix: A Hybrid Approach to Personalized Movie Recommendations

## Overview
HybridFlix is a movie recommendation system that combines content-based and collaborative filtering techniques to provide personalized movie suggestions. This project leverages the TMDB movie dataset to enhance user experience by recommending movies based on both content attributes and user ratings.

## Features
- **Content-Based Recommendations**: Utilizes movie features such as genre, keywords, and overview to suggest similar movies.
- **Collaborative Filtering**: Analyzes user ratings and popularity to recommend movies that are well-received by similar users.
- **Hybrid Recommendations**: Combines both content-based and collaborative filtering results for a more robust recommendation system.
- **Evaluation Metrics**: Implements metrics such as similarity, diversity, novelty, and NDCG (Normalized Discounted Cumulative Gain) to assess the quality of recommendations.
- **Visualization**: Provides visual insights into the performance of different recommendation methods using heatmaps.

## Installation
To run this project, you need to have Python installed along with the following libraries:
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn

You can install the required libraries using pip:
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

## Usage
1. **Data Preparation**: Ensure you have the TMDB movie dataset CSV files (`tmdb_5000_credits.csv` and `tmdb_5000_movies.csv`). Place them in the appropriate directory.
2. **Run the Notebook**: Open the Jupyter Notebook and execute the cells to load the data, train the recommendation models, and generate movie recommendations.
3. **Get Recommendations**: Use the `get_recommendations` method to find movie suggestions based on a specific movie title.

### Example
```python
recommender = EnhancedMovieRecommender()
recommender.fit('path/to/tmdb_5000_credits.csv', 'path/to/tmdb_5000_movies.csv')
content_recs, collab_recs, hybrid_recs = recommender.get_recommendations("The Dark Knight")
```

## Evaluation
To evaluate the performance of the recommendation system, run the `evaluate_recommendations` method. This will provide insights into the effectiveness of each recommendation strategy.

## Visualization
Use the `plot_evaluation_results` method to visualize the evaluation metrics in a heatmap format, allowing for easy comparison between different recommendation methods.

## Contributing
Contributions are welcome! If you have suggestions for improvements or new features, feel free to open an issue or submit a pull request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
- TMDB (The Movie Database) for providing the movie dataset.
- The open-source community for the libraries used in this project.

## Contact
For any inquiries, please reach out via GitHub or email.

---

Feel free to modify any sections to better fit your project's specifics or personal preferences!
