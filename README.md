# Movie Recommendation System

A Streamlit movie browser and FastAPI recommendation backend. Movie metadata and
recommendations are fetched from TMDB; similar-movie results also use the
included local TF-IDF model files.

## Setup

1. Install dependencies with `pip install -r requirements.txt`.
2. Create a `.env` file containing a TMDB-issued API key:

   ```text
   taste_dive_api_key=your_tmdb_api_key
   ```

3. Start the API from this directory:

   ```text
   uvicorn main:app --reload
   ```

4. In a separate terminal, start the Streamlit app:

   ```text
   streamlit run appy.py
   ```

The `.env` file is local-only and must not be committed. The key variable keeps
the existing project name, but its value must be issued by TMDB.
