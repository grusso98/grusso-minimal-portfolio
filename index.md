# Portfolio
---

## Data Science for Cybersecurity

### Master Thesis: Unsupervised Machine Learning for Intrusion Detection Systems.

[![View on GitHub](https://img.shields.io/badge/GitHub-View_on_GitHub-blue?logo=GitHub)](https://github.com/grusso98/Unsupervised_Intrusion_Detection/tree/main)
[![Open PDF](https://img.shields.io/badge/PDF-View%20Report%20Pdf-red?logo=adobe-acrobat-reader)](https://github.com/grusso98/Unsupervised_Intrusion_Detection/blob/main/Thesis.pdf)

<div style="text-align: justify">
<b>ML Intrusion Detection</b> implemented using Autoencoders, One Class SVM and Isolation Forest.
<br> <br>
This thesis explores anomaly detection of web-based attack on microservices based applications by modeling application performance metrics and service logs. The general idea is that a normal activity profile can be built upon the (simulated) normal activity on the web application and then the anomalies such as web attacks can be detected as different behaviour with respect to the normal activity. This task will be carried out by generating a dataset only containing normal activity and then train machine learning models to distinguish between the learnt behaviour and different behaviours.
</div>
<br>
<center><img src="images/ids.png"/></center>
<br>


### Adversarial Attacks in Deep Learning Systems.

[![View on GitHub](https://img.shields.io/badge/GitHub-View_on_GitHub-blue?logo=GitHub)](https://github.com/grusso98/Cybersecurity_for_Data_Science)
[![Open PDF](https://img.shields.io/badge/PDF-View%20Report%20Pdf-red?logo=adobe-acrobat-reader)](https://github.com/grusso98/Cybersecurity_for_Data_Science/blob/main/Cybersec_Report.pdf)

<div style="text-align: justify">
<b>Adversarial Attack detection</b> using SVD as a proactive measure.
<br> <br>
<h4>Brief description</h4>
<p>Machine learning models, crucial in various applications like autonomous driving and security systems, are vulnerable to adversarial attacks. These attacks manipulate data to degrade model performance or breach confidentiality.</p>
<p><b>Fast Gradient Sign Method (FGSM)</b> and <b>Projected Gradient Descent (PGD)</b> are two prominent adversarial techniques. FGSM performs one-step updates to maximize loss, while PGD is an iterative, robust version of FGSM.</p>
<p>Defensive strategies include <b>denoising</b> to clean inputs and <b>Singular Value Decomposition (SVD)</b> to reduce dimensionality and remove perturbations. Practical demonstrations using the CleverHans library showcased these methods on datasets like MNIST.</p>
<p>While these defenses are effective, they require access to training data and can be computationally intensive, especially for large datasets.</p>

</div>
<br>
<center><img src="images/fgsm.png"/></center>
<br>

---

## Computer Vision and Signals 

### Image and Audio SuperResolution using CNN and GANs.

[![View on GitHub](https://img.shields.io/badge/GitHub-View_on_GitHub-blue?logo=GitHub)](https://github.com/grusso98/DSIM)
[![Open PDF](https://img.shields.io/badge/PDF-View%20Report%20Pdf-red?logo=adobe-acrobat-reader)](https://github.com/grusso98/DSIM/blob/master/DSIM%20Presentation.pdf)

<div style="text-align: justify">
<b>CNN</b> and <b>GANs</b> for super resolution.
<br> <br>
The main objective is to train Convolutional Neural Networks and Generative Adversarial Network for the task of super resolution: the enhancement of 1D (audio) and 2D(images) signals. This repository contains the demo that uses our trained models to apply super resolution to images and audio.
</div>
<br>
<center><img src="images/SR.png"/></center>
<br>

---
### Pill Quality Control / Classification and Augmentation.

[![View on GitHub](https://img.shields.io/badge/GitHub-View_on_GitHub-blue?logo=GitHub)](https://github.com/grusso98/Foundations_of_Deep_Learning)
[![Open PDF](https://img.shields.io/badge/PDF-View%20Report%20Pdf-red?logo=adobe-acrobat-reader)](https://github.com/grusso98/Foundations_of_Deep_Learning/blob/main/PillQC-FDL.pdf)

<div style="text-align: justify">
<b>Image classification</b> and <b>augmentation</b> using traditional techniques and Generative Adversarial Neural Networks.
<br> <br>
The first objective of this project is to perform classification on pills, specifically trying to detect if in a quality control scenario is possibile to detect pills with cosmetics defects like chips or dirt. This task has been carried out training CNNs from scratch and comparing them with pre-trained nets.
The second objective is to remedy for the lack of training data using generative adversarial neural networks (GANs), combined with traditional data augmentation.
</div>
<br>
<center><img src="images/pil.gif"/></center>
<br>

---
## Natural Language Processing
### AppointMate: Appointment Agent App.
<center>
  <img src="https://raw.githubusercontent.com/grusso98/AppointMate/main/imgs/appointmate_logo.png" alt="Chat Interface" width="100%">
</center>

[![View on GitHub](https://img.shields.io/badge/GitHub-View_on_GitHub-blue?logo=GitHub)](https://github.com/grusso98/AppointMate)

A conversational AI agent built with LangChain that allows users to book appointments with a professional via Telegram. The agent can check availability based on a schedule stored in an SQLite database and confirm bookings, optionally sending email notifications.

#### Functionalities

* **Conversational Interface:** Interacts with users naturally through Telegram.
* **Availability Checking:**
    * Understands natural language date queries (e.g., "today", "tomorrow", "next Friday", "July 10th") using `dateparser`.
    * Consults an SQLite database for existing appointments.
    * Checks against predefined working hours.
    * Presents available time slots to the user.
* **Appointment Booking:**
    * Guides the user to select a specific available slot.
    * Prompts the user for their name if not already provided in the conversation.
    * Saves the confirmed appointment to the SQLite database, preventing double booking.
* **Edit Appointments:**
    * Allows the user to edit exisiting appointment, checking for available slots.
* **LLM Integration:** Supports using different Language Models:
    * OpenAI models (e.g., GPT-4o-mini) via API.
    * Local models via Ollama (e.g., Llama 3).
* **(Optional) Email Notifications:**
    * Sends a confirmation email to the professional upon successful booking.
    * Attaches an `.ics` calendar invite file for easy addition to calendars (like Google Calendar, Outlook).
    * Requires SMTP configuration in the `.env` file to function.

### RAGademic: LLM+RAG for your notes.
<center>
  <img src="https://raw.githubusercontent.com/grusso98/RAGademic/main/imgs/ragademic_logo.png" alt="Chat Interface" width="100%">
</center>

[![View on GitHub](https://img.shields.io/badge/GitHub-View_on_GitHub-blue?logo=GitHub)](https://github.com/grusso98/RAGademic)

<div style="text-align: justify">
This project provides a <b>Retrieval-Augmented Generation (RAG) system</b> to query your university notes and books efficiently (could be used to retrieve any kind of document really, but this is the use case I've opted for! :) ). It allows users to upload PDF documents, store them in a <b>Chroma vector database</b>, and interact with them through an <b>LLM-powered chatbot</b>. The project also includes a visualization tool for document embeddings.

<h4>Features</h4>
<ul>
  <li><b>Chat with your notes</b>: Ask questions, and the system retrieves relevant information using embeddings.</li>
  <li><b>Database management</b>: Upload, delete, and visualize document embeddings.</li>
  <li><b>Arxiv source addition</b>: Search for papers on specific topics and add them to your knowledge base.</li>
  <li><b>Three LLM options</b>:
    <ul>
      <li>Use <b>OpenAI's API</b></li>
      <li>Use local models like <b>LLaMA3.2</b></li>
      <li>Use the new <b>Gemma3</b> via ollama chat</li>
    </ul>
  </li>
  <li><b>Three Embedding options</b>:
    <ul>
      <li>Use <b>OpenAI's embedder</b></li>
      <li>Use <b>HF embedder</b> from the hub</li>
      <li>Use <b>chroma builtin local embedder</b></li>
    </ul>
  </li>
  <li><b>Persistent memory</b>: Keeps track of conversations in between sessions, using llama3.2 as a summarizer to keep context windows occupation optimized.</li>
  <li><b>Web Search Agent</b>: If activated, it evaluates (using local llama3.2) the pertinence of the local knowledge wrt the query of the user and if necessary it scrapes the web for more context.</li>
</ul>
<br>
</div>
<center>
  <img src="https://raw.githubusercontent.com/grusso98/RAGademic/main/imgs/chat.png" alt="Chat Interface" width="100%">
</center>
<br>
<center>
  <img src="https://raw.githubusercontent.com/grusso98/RAGademic/main/imgs/db_management.png" alt="DB Management Interface" width="100%">
</center>
<br>
<center>
  <img src="https://raw.githubusercontent.com/grusso98/RAGademic/main/imgs/embedding_viz.png" alt="Embeddings Visualization" width="100%">
</center>

### NIPS Papers: Topic Modelling and Text Summarization.

[![View on GitHub](https://img.shields.io/badge/GitHub-View_on_GitHub-blue?logo=GitHub)](https://github.com/grusso98/Text-Mining)
[![Project Report](https://img.shields.io/badge/PDF-Project%20Report-red?logo=adobe-acrobat-reader&logoColor=white)](https://github.com/grusso98/Text-Mining/blob/main/Report.pdf)

<div style="text-align: justify">
The Neural Information Processing System (NIPS) is a machine learning and computational neuroscience competition held every year from 1987 to date. We tackled a dataset containing all the papers submitted from 1987 to 2017, with the aim of applying unsupervised NLP models for topic modelling (LDA/PLSA) and a supervised approach for extractive text summarization (topic representation and indicator representation).
<br> <br>
</div>
<br>
<center><img src="images/tm.png"/></center>
<br>

---
### 7 Sins Diachronical Analysis
[![View on GitHub](https://img.shields.io/badge/GitHub-View_on_GitHub-blue?logo=GitHub)](https://github.com/grusso98/Data_Semantics)
[![Open PDF](https://img.shields.io/badge/PDF-Project%20Report%20Paper-red?logo=adobe-acrobat-reader)](https://github.com/grusso98/Data_Semantics/blob/main/Seven%20Deadly%20Sins_Chiriaco_Porcedda_Russo.pdf)

<div style="text-align: justify">
The aim of the work is to perform a diachronic analysis of the 7 deadly sins to find out how their meaning and use has changed from the 19th century to the 21st century. Additionally, we tried implementing some comparison metrics for the embedding models we used.
<br>
This work involved using different word embedding techniques: Word2Vec and GloVe, while using CADE to align the text corpora and analyze the semantic difference of the words between the 1800s and 2000s. Additionally, we implemented a geometrical comparison technique to evaluate how different the embeddings are built between W2V and GloVe.
</div>
<br>
<center><img src="images/DS-banner.png"/></center>
<br>

---

## Time Series Analysis

### Restaurant's Revenue Loss during first COVID-19 pandemic lockdown (ITA).

[![View on GitHub](https://img.shields.io/badge/GitHub-View_on_GitHub-blue?logo=GitHub)](https://github.com/grusso98/Data_Science_Lab)
[![Open PDF](https://img.shields.io/badge/PDF-View%20Report%20Pdf-red?logo=adobe-acrobat-reader)](https://github.com/grusso98/Data_Science_Lab/blob/main/Report_PorceddaChiriacoRusso.pdf)

<div style="text-align: justify">
<b> Time Series </b> Analysis and <b> Forecasting </b> (using <b> ARIMA </b>, and <b> Mixture models </b>) of a <b> restaurant's revenue </b> during the first lockdown of the COVID-19 pandemic in Italy, to estimate the loss incurred..
<br> <br>
One of the sectors most affected by the Covid-19 pandemic has certainly been the restaurant industry. Due to the related restrictions, restaurant owners saw their revenues plummet dramatically. In such a historical period, it can be very useful to analyze historical data to try to study and predict what the daily or weekly revenues will be in order to adjust the supply of raw materials accordingly. In this paper, models from the ARIMA family and the Cluster-Weighted Model with and without cross-validation were used for forecasting time series.
</div>
<br>
<center><img src="images/covid-restaurant.png"/></center>
<br>

---

### Energy Consumption Forecast (ITA).

[![View on GitHub](https://img.shields.io/badge/GitHub-View_on_GitHub-blue?logo=GitHub)](https://github.com/grusso98/SDMTSA)
[![Open PDF](https://img.shields.io/badge/PDF-View%20Report%20Pdf-red?logo=adobe-acrobat-reader)](https://github.com/grusso98/SDMTSA/blob/main/SDMTSA_887277.pdf)

<div style="text-align: justify">
<b> Time Series </b> Analysis and <b> Forecasting </b> (using <b> ARIMA </b>, <b> UCM </b> and <b> LSTMs </b> models) of <b>energy consumption</b>. 
<br> <br>
Energy consumption forecasts are crucial for various purposes, from purchasing energy from the producer to managing overloads. This paper analyzes a univariate time series of energy consumption sampled every 10 minutes. The provided period spans from 01/01/2017 to 30/11/2017, with the aim of estimating December's consumption. The dataset, in total, consists of 48,096 observations. There are no additional details such as weather, holidays, and other typical location-specific characteristics.
</div>
<br>
<center><img src="images/sdmtsa.png"/></center>
<br>

---


## Data Visualization

### Netflix Top 10 Quality: Data Analysis & Interactive Visualization (ITA).

[![View on GitHub](https://img.shields.io/badge/GitHub-View_on_GitHub-blue?logo=GitHub)](https://github.com/grusso98/Netflix-Top10-Quality)
[![View on Tableau](https://img.shields.io/badge/Tableau-View_on_Tableau-orange?logo=Tableau)](https://rporcedda.github.io/Netflix-Top10-Quality/)


<div style="text-align: justify">Netflix calculates the "Weekly Top 10" simply by ordering movies or TV series based on the hours viewed in the last 7 days in descending order. But <b>does this ranking truly reward titles of higher quality or the most popular ones</b>? Are <b>movies and TV series treated equally</b>? <b>Is the Top 10 genuinely helpful</b> for users in selecting the best titles, or does it feature lower-quality content compared to what is available in Netflix's catalog?
<br>
Netflix is one of the most widely used streaming platforms, boasting over 214 million accounts. The platform employs one of the most effective recommendation systems, featuring on each user's homepage the most popular movies and TV series that align with the subscriber's preferences.

A common feature among all accounts is the "Weekly Top 10," which appears at the top of the homepage and is updated every Sunday. Millions of people see this list of the top ten movies or TV series every day, inevitably influencing users' choices. Furthermore, it serves as an invaluable showcase for every actor and director, both emerging and established.

The objective of this research is to analyze data related to each movie and TV series that made it into the Top 10 in the last six months to answer these research questions.
</div>
<br>
<center><img src="images/dataviz1.png"/></center>
<br>

---
### Infographics: PROM score and the possible relationship with weather conditions (ITA).


<div style="text-align: justify">
<b>PROMs are patient-reported outcome</b> measures following an operation or health treatment, often used to assess the quality of health care.
<br>
We evaluated, through some <b>infographics</b> made through Python, using the <b>matplotlib</b> and <b>Seaborn</b> libraries, the possible presence of a <b>relationship</b> between the <b>outcomes of mental and physical health status assessments</b> of a sample of patients, following surgery, and the <b>gender and time(day and night)</b> relative to the time of questionnaire completion.
</div>
<br>
<center><img src="images/dataviz2.png"/></center>
<br>

---
## Data Management

### Data Acquisition and Modeling: Movies and Tv series using Netflix and IMDB Data (ITA).

[![Open PDF](https://img.shields.io/badge/PDF-Read%20%20Report%20%20PDF-red?logo=adobe-acrobat-reader)](https://github.com/grusso98/Netflix-Top10-Quality/blob/main/882638_886719_887277_DM.pdf)

<div style="text-align: justify">
Data Acquisition and Modeling: <b>Document-based database</b> containing information related to <b>IMDB and Netflix</b>, <b>scraped</b> from various sources and obtained via <b>API</b>.
<br> <br>
The following study focuses on the acquisition, aggregation, integration, cleaning, and storage of a series of datasets related to the Netflix streaming platform in MongoDB. In particular, various data acquisition techniques such as web scraping and APIs were employed. Once the necessary data to answer research questions were obtained, they underwent cleaning and enrichment. Dozens of attributes related to titles that made it into Netflix's weekly Top 10 were derived from data provided by IMDb. Through the comprehensive enrichment process, a more enriched dataset with a more "flexible" structure was obtained and stored in the document-based MongoDB database.
</div>
<br>
<center><img src="images/mongodb.png"/></center>
<br>

<center>© 2023 Russo Gianmarco. Powered by Jekyll and the Minimal Theme.</center>