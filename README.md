# **PlotEmbed**  
**Efficient Sentence Embedding and Aggregation for Plot Descriptions**

---

## **Description**
PlotEmbed is a Python-based project designed to generate embeddings for plot descriptions using transformer models. It processes textual data (such as movie plots, book summaries, or other descriptive narratives), splits them into sentences, encodes each sentence into high-dimensional embeddings using a Sentence Transformer, and aggregates these embeddings to create a single representation for the entire plot.

The project is particularly useful for tasks such as:
- **Semantic similarity** between plots.
- **Clustering or categorization** of textual narratives.
- **Text-based recommendation systems**.

---
**Dataset**: https://studentuml-my.sharepoint.com/:u:/g/personal/svarrajankumar_patel_student_uml_edu/ER9ocuVQx7xAmDeAmEYxpJoBfc-5ogpgF0tyG-h3_D5wvA?e=sakAMK

---

## **Features**
- **Sentence Tokenization**: Breaks plots into individual sentences for better handling of context.
- **Sentence Capping**: Limits the number of sentences per plot to ensure efficient processing and memory management.
- **Sentence Encoding**: Uses pre-trained transformer models to generate embeddings for each sentence.
- **Plot-Level Embedding**: Aggregates sentence embeddings using sum or mean pooling to create a comprehensive plot representation.
- **Progress Tracking**: Provides a detailed progress bar for various stages of computation, making it easy to monitor large-scale processing.

---

## **How It Works**
1. **Input**: A DataFrame containing plot descriptions.
2. **Processing**:
   - Sentences are tokenized and optionally capped to a specified limit.
   - Sentence embeddings are generated using a transformer model.
   - Plot embeddings are computed by aggregating sentence-level embeddings.
3. **Output**: A list of vectorized embeddings, one for each plot, ready for downstream tasks like similarity computation or classification.

## **Applications**
- **Recommendation Systems**: Generate embeddings for personalized recommendations.
- **Semantic Search**: Create searchable databases of text with vector similarity.
- **Clustering**: Group plots or texts by similarity for categorization or exploration.

---

## **To-Do**
- [ ] Add support for custom transformer models.
- [ ] Incorporate GPU-based acceleration for large datasets.
- [ ] Support additional pooling techniques for aggregation.
- [ ] Explore other tokenization techniques for better preprocessing.
