# Book-Recommendation-System-Collaborative-Filtering-at-Scale
Book Recommendation System : Collaborative Filtering at Scale

Built a scalable, personalized book recommendation engine using User-Based Collaborative Filtering on a large real-world dataset (Ratings.csv, Books.csv).

• Engineered a user-item matrix using SciPy sparse matrices (CSR format) and exported it in LIBSVM format for ML compatibility; cosine similarity was used to identify the top-10 most similar users per target user.
• Designed a batch-based similarity pipeline processing users in chunks of 1,000 to handle memory constraints at scale generating 210,000+ personalized book recommendations across the full dataset.
• Implemented a weighted similarity scoring model to estimate ratings for unseen books, filtering already-rated titles and invalid ISBNs to ensure recommendation quality.
• Conducted end-to-end data preparation including deduplication, sparse matrix construction, and structured CSV output with user ID, book title, and recommendation scores.

Tech: Python · Pandas · NumPy · SciPy · scikit-learn · Collaborative Filtering · Sparse Matrices · LIBSVM
