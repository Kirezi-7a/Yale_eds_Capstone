# Yale_eds_Capstone
Capstone project for Yale EDS Online Program, analysing environmental change using text data for quantitative analysis
# Project Title
Understanding how Forest and land-based carbon projects' impact on indigenous communities is reported across different documentations
# Research Question
What are the thematic differences in how carbon credits and community impacts are discussed in official project documentation vs independent reporting for the Northern Kenya Rangelands Carbon Project?
# Why this project matters
Carbon credit projects are not new to criticism around their real impact and how they truly benefit the communities involved. One of the most talked about concerns is carbon credit project reporting integrity, where some projects have appeared to be untruthful about carbon emissions prevented and the true impact on communities. In this project, we specifically looked at the Northern Kenya Rangeland Carbon Project and compared how the official documentation, specifically monitoring reports submitted to the certifying body, Verra Registry, differs from independent reporting on community impact and how the indigenous communities in Northern Kenya have been affected by the project. For the **Northern Kenya Rangelands Carbon Project**, this difference matters because the project operates in pastoralist areas where grazing practices, land governance, and benefit sharing directly affect local communities.As carbon markets continue to expand across Africa, governments will play a bigger role in deciding how these projects are approved, monitored, and governed. Looking at the gap between official and independent reporting can help show whether current project narratives fully reflect what is happening on the ground.
# Audience
This project is mainly intended for:
- Government officials  
- Carbon credit certifying bodies  
- Policy makers  
It may also be useful for researchers, civil society organisations, and others interested in carbon markets, land governance, and climate justice.
# Data
For this Capstone, I am working with a **text-based dataset** that I compiled for analysing thematic differences in how carbon credits and community impacts are discussed across independent and official project documentation sources.
# Dataset
**Northern Kenya Rangelands Carbon Project Text Corpus (5 documents)**  
A CSV containing official NRT project documentation and independent investigative reporting.
# Official project documents
- Two monitoring reports covering the period of 2017-2021
# Independent sources**
- 3 independent reports and an article about the project.
All documents are converted to text format and organised into a CSV file for analysis.
 # Data Structure
The dataset includes the following key variables:
- **source** – categorical variable identifying whether the document is **“official”** or **“independent”**
- **year** – publication year
- **doc_id** – document identifier
- **doc_name** – name of the original report or article
- **text** – unstructured document text
# Process (Metacode)
My workflow follows a basic text analysis pipeline in R.
# Step 1: Import data
- Load the CSV file into R
- Inspect variables and document structure
# Step 2: Clean and preprocess text
- Convert text to lowercase
- Tokenise text into individual words
- Remove punctuation and extra whitespace
- Remove standard stopwords
- Remove domain-specific high-frequency words that do not add thematic meaning (for example: “project,” “carbon,” “NRT”)
# Step 3: Explore the data
- Compare document lengths by source
- Count words after cleaning
- Generate word frequencies
- Identify early framing differences between official and independent documents by highlighting words that appear more frequently in one set of documents than the other
# 4. Structural Topic Modelling (STM) 
At this stage, I used STM to identify the main themes that emerge across the text and to examine whether those themes differ depending on whether the source is **official** or **independent**.
# STM workflow includes:
- preparing the cleaned text in a format suitable for STM
- fitting the topic model
- selecting and interpreting the number of topics
- examining top words per topic
- comparing topic prevalence across source types
# Step 5: Visualise findings
- Produce summary tables and visualisations to show thematic patterns and differences in framing
- I also mapped the overall area covered by the Northern Kenya Rangelands Carbon Project

# Key Findings
This project examined how official and independent documents frame carbon credits and community impacts in the Northern Kenya Rangelands Carbon Project. Using TF-IDF, Structural Topic Modelling, and spatial visualisation, I found that official sources emphasise project metrics and reported benefits, while independent sources foreground community experience, land rights, conflict, and place.
# Author
Ikirezi Anitha
