---
title: "Project 1 Progress: Classification Results and Feature Experimentation"
date: 2026-08-05
permalink: /posts/2026/08/project-1-week-6-7/
reading_time: "2 min read"
tags: AI bootcamp research arXiv SPARK classification
---

After completing the classification notebook, I built and trained a neural network classifier on the 1000 arXiv papers using the five extracted features. The model was a three-layer network designed to predict each paper's primary category from task, method, dataset, metric, and domain. Results showed 50% test accuracy across 76 categories, which raised an important question: the baseline of always guessing the most common category achieved 57% accuracy, meaning the extracted features alone were not carrying enough signal to be useful.

This finding was honest and valuable. Rather than accepting it as failure, I calculated additional metrics including macro-F1, precision, and recall per class, which revealed that the model had learned to predict almost everything as the dominant category. The low macro-F1 score reflected severe class imbalance in the dataset. I documented these results in a four-page LaTeX report using Overleaf, including a confusion matrix and training curves that showed the model did learn during training even though the test performance was weak.

With the classification results documented, I tested alternative approaches to improve the signal. I experimented with different feature representations and encoding methods, including TF-IDF vectorization on full abstracts, which a teammate had applied with much stronger results (83.5% accuracy). This comparison showed that using all the words from paper abstracts, rather than extracting five specific fields, captured far more useful information for category prediction.

The takeaway reshaped how I think about the knowledge graph: extracted features are a starting point, but combining them with text-based approaches will likely produce better results. The coming weeks will involve building the knowledge graph using these insights, exploring how to connect papers based on both structured features and semantic similarity from their full text.

