

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  
</head>
<body>

<h1>📩 SMS Spam Classifier with NLP</h1>

<p>This project demonstrates how to build a simple spam detection model using <strong>Natural Language Processing (NLP)</strong> techniques and machine learning. The goal is to accurately classify SMS messages as either <code>ham</code> (not spam) or <code>spam</code>.</p>

<h2>📂 Dataset</h2>
<p>The dataset consists of labeled SMS messages with two columns:</p>
<ul>
  <li><strong>Class:</strong> Label indicating if the message is <em>spam</em> or <em>ham</em>.</li>
  <li><strong>Message:</strong> The text content of the SMS.</li>
</ul>

<h2>🚀 Workflow Overview</h2>
<ol>
  <li><strong>Data Loading:</strong> Read the dataset using pandas, check for null values, and explore class distribution.</li>
  <li><strong>Text Preprocessing:</strong> 
    <ul>
      <li>Convert text to lowercase</li>
      <li>Remove special characters using regular expressions</li>
      <li>Remove stopwords</li>
      <li>Apply stemming using PorterStemmer</li>
    </ul>
  </li>
  <li><strong>Feature Extraction:</strong> Two different techniques were applied:
    <ul>
      <li>Bag of Words (BoW)</li>
      <li>TF-IDF (Term Frequency–Inverse Document Frequency)</li>
    </ul>
  </li>
  <li><strong>Model Training:</strong> Split the data (80/20) and trained two models:
    <ul>
      <li>Multinomial Naive Bayes</li>
      <li>Logistic Regression</li>
    </ul>
  </li>
  <li><strong>Prediction & Evaluation:</strong> Used both models to predict and evaluate results using a confusion matrix.</li>
</ol>

<h2>🧠 Models Used</h2>
<ul>
  <li><strong>Multinomial Naive Bayes:</strong> Fast and efficient for text classification tasks.</li>
  <li><strong>Logistic Regression:</strong> Also used for comparison with TF-IDF features.</li>
</ul>

<h2>📊 Evaluation</h2>
<p>After training, predictions were evaluated using <strong>confusion matrices</strong> for each model and feature extraction method. This helped in understanding the performance in terms of false positives, true negatives, etc.</p>

<h2>🔧 Requirements</h2>
<pre>
pandas
numpy
matplotlib
scikit-learn
nltk
</pre>

<h2>📝 Notes</h2>
<p>Stemming was used instead of lemmatization for simplicity. If you want more linguistic accuracy, consider using <code>WordNetLemmatizer</code>.</p>

<h2>📌 Conclusion</h2>
<p>This project shows how you can quickly build a text classification pipeline using basic NLP and machine learning techniques. Both Bag of Words and TF-IDF perform well, with TF-IDF generally providing a slight performance improvement.</p>

</body>
</html>
