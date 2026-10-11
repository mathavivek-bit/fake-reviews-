# Fake Review Detector (mini project)

Full-stack Java project (no external libraries): Java backend + HTML/CSS/JS frontend.
Detection = Naive Bayes classifier + rule-based red flags (hype words, links, duplicates, rating mismatch, etc.).

## Structure
```
backend/   Main.java (REST server) | ReviewAnalyzer.java | NaiveBayes.java | TrainingData.java | Demo.java
frontend/  index.html | style.css | app.js
```

## Run the web app
```
cd backend
javac *.java
java Main
```
Open http://localhost:8080

## Run the console demo (prints output in the terminal)
```
cd backend
javac *.java
java Demo
```

## API
- POST /api/analyze  body: {"review": "text", "rating": 5}
- GET  /api/history

Requires JDK 17+.
