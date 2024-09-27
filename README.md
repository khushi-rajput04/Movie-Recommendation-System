# Movie Recommendation System

A content-based movie recommendation system that suggests movies based on user preferences. This project leverages machine learning techniques to recommend movies by analyzing key features like genres, cast, and keywords from a dataset of over 4800 movies.

## Features

- **Content-based filtering**: Recommends movies based on similarity in features such as genres, cast, crew, and keywords.
- **Efficient similarity algorithm**: Uses `CountVectorizer` and `Cosine Similarity` to generate and rank recommendations.
- **Interactive user interface**: Built with `Streamlit` to allow users to search and receive recommendations easily.
- **Real-time data**: Integrates with the TMDB API to retrieve additional movie details.

# Website

![screenshot1](https://github.com/khushi-rajput04/Movie-Recommendation-System/blob/main/screenshot1.png)

![screenshot2](https://github.com/khushi-rajput04/Movie-Recommendation-System/blob/main/screenshot2.png)

![screenshot3](https://github.com/khushi-rajput04/Movie-Recommendation-System/blob/main/screenshot3.png)


## Tech Stack

- **Frontend**: HTML, CSS (via Streamlit)
- **Backend**: Python, Pandas
- **API**: TMDB API for movie metadata
- **Libraries**:
  - `Pandas`: For data manipulation and processing
  - `Scikit-learn`: For vectorization and similarity calculation
  - `Streamlit`: For web interface
  - `Numpy`: For numerical operations

## How It Works

1. **Data Preprocessing**:
   - Movie metadata like `genres`, `cast`, `crew`, and `keywords` are combined into unified "tags" for each movie.
   
2. **Vectorization**:
   - The movie tags are vectorized using `CountVectorizer`, which converts text data into a matrix of token counts.

3. **Similarity Calculation**:
   - Cosine similarity is computed between the vectors to determine how similar two movies are based on their tags.

4. **Recommendations**:
   - For a selected movie, the system ranks other movies based on their similarity score, returning the top matches.

## Installation

### Prerequisites

Ensure you have the following installed:

- Python 3.x
- `pip` (Python package installer)

### Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/movie-recommendation-system.git
   ```

2. Navigate to the project directory:
   ```bash
   cd movie-recommendation-system
   ```

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Run the Streamlit app:
   ```bash
   streamlit run app.py
   ```

## Usage

1. Launch the web app using Streamlit.
2. Enter the name of a movie in the search bar.
3. The system will generate a list of similar movies based on the selected movie’s tags.
