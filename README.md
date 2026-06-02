# 🏏 IPL Match Simulation using Monte Carlo Method

> ⚠️ **Disclaimer:** This project uses Monte Carlo Simulation with random number generation. Match outcomes, team scores, wickets, and KPI metrics may vary across simulation runs due to the probabilistic nature of the model.

---

## 📌 Project Overview

This project implements an **IPL Match Simulation Model** using the **Monte Carlo Method** in **Google Sheets**. The simulation predicts match outcomes through a ball-by-ball probabilistic approach by leveraging historical IPL player performance data.

The model computes batting and bowling event probabilities from historical statistics and simulates complete innings to estimate match results, team performance metrics, and win probabilities.

The project demonstrates the practical application of probability theory, statistical modeling, and simulation techniques in sports analytics.

---

## 🎯 Objective

The primary objective of this project is to:

* Simulate IPL matches on a ball-by-ball basis using probabilistic outcomes.
* Predict match results based on historical player performance.
* Estimate team win probabilities through repeated simulations.
* Analyze batting and bowling performance using data-driven insights.

---

## 🛠 Methodology

### 1. Data Preparation

Historical IPL player statistics were collected and organized into batting and bowling datasets.

#### Batting Statistics

* Balls Faced
* Dot Balls
* Singles (1s)
* Doubles (2s)
* Triples (3s)
* Fours (4s)
* Sixes (6s)
* Dismissals

#### Bowling Statistics

* Balls Bowled
* Wides
* No Balls
* Wickets

---

### 2. Probability Calculation

Player-specific probabilities were calculated using historical data.

**Formula:**

```text
P(Event) = Event Count / Total Balls
```

Examples:

* Probability of a Dot Ball
* Probability of scoring 1 Run
* Probability of scoring 2 Runs
* Probability of scoring 4 Runs
* Probability of scoring 6 Runs
* Probability of Dismissal
* Probability of Wide Ball
* Probability of No Ball

Cumulative probability distributions were then generated to facilitate random event selection during simulations.

---

### 3. Monte Carlo Simulation Engine

For each ball:

1. Generate a random number between 0 and 1.
2. Compare the generated value against cumulative probability ranges.
3. Determine the outcome:

   * Dot Ball
   * 1 Run
   * 2 Runs
   * 3 Runs
   * 4 Runs
   * 6 Runs
   * Wicket
   * Wide
   * No Ball
4. Update:

   * Team Score
   * Balls Remaining
   * Wickets
   * Batting Order

The innings continues until:

* 20 overs are completed, or
* All wickets are lost.

---

### 4. Match Simulation

The model performs:

* Toss Simulation
* First Innings Simulation
* Target Generation
* Second Innings Chase Simulation
* Winner Determination

Multiple iterations are executed to estimate realistic win probabilities.

---

## 📊 Features

### Batting Simulation

* Player-specific scoring probabilities
* Dynamic batting order management
* Strike rotation
* Boundary frequency analysis

### Bowling Simulation

* Wide ball probabilities
* No-ball probabilities
* Wicket-taking probabilities
* Bowling performance evaluation

### Match Engine

* Toss simulation
* Innings progression
* Score tracking
* Wicket tracking
* Match outcome prediction

### KPI Dashboard

The dashboard provides:

* Total Runs Scored
* Total Wickets Taken
* Maximum Runs Scored
* Maximum Wickets Taken
* Dot Balls
* Fours (4s)
* Sixes (6s)
* Extras (Wides + No Balls)
* Win Probability (%)

---

## 📁 Project Structure

### PBKS Sheet

Contains:

* Playing XI
* Batting probability calculations
* Bowling probability calculations
* Player performance statistics

### KKR Sheet

Contains:

* Playing XI
* Batting probability calculations
* Bowling probability calculations
* Player performance statistics

### Simulation Sheet

Contains:

* Ball-by-ball simulation logic
* Random number generation
* Match calculations
* Score and wicket updates

### KPI Sheet

Contains:

* Match summary
* Team comparison metrics
* Performance indicators
* Win probability analysis

---

## 📈 Sample Output

| Metric                | PBKS   | KKR    |
| --------------------- | ------ | ------ |
| Total Runs Scored     | 582    | 649    |
| Total Wickets         | 30     | 23     |
| Maximum Runs Scored   | 155    | 155    |
| Maximum Wickets Taken | 8      | 9      |
| Win Probability (%)   | 42.86% | 57.14% |

---

## ⚠️ Important Note on Simulation Results

Since this project uses **Monte Carlo Simulation**, the results are generated using random values based on historical probability distributions.

Therefore:

* KPI values may change every time the simulation is executed.
* Match scores, wickets, and outcomes are not deterministic.
* Different simulation runs may produce different results even with the same input data.
* The displayed metrics represent probabilistic estimates rather than exact predictions.
* Increasing the number of simulation iterations improves the stability and reliability of win probability estimates.

> **Note:** Any refresh, recalculation, or rerun of the model may generate slightly different KPI values and match outcomes.

---

## 👨‍💻 Roles & Responsibilities

* Utilized historical IPL ball-by-ball datasets to derive player-specific probability distributions.
* Computed cumulative probabilities for batting and bowling outcomes using Google Sheets formulas.
* Designed and implemented a Monte Carlo-based ball-by-ball simulation framework.
* Developed toss logic and innings progression mechanisms.
* Performed data cleaning, preprocessing, and validation.
* Generated match-level insights and KPIs through repeated simulations.
* Created dashboards for performance analysis and win probability visualization.

---

## 💻 Technologies Used

* Google Sheets
* Monte Carlo Simulation
* Probability Theory
* Statistical Analysis
* Sports Analytics

---

## 📚 Key Learnings

* Monte Carlo Simulation Techniques
* Probability Distribution Modeling
* Cricket Analytics
* Statistical Forecasting
* Spreadsheet-Based Simulation Design
* Data-Driven Decision Making

---

## 🚀 Future Enhancements

* Incorporate venue-specific statistics.
* Add pitch and weather condition effects.
* Include recent player form and performance trends.
* Integrate machine learning models for probability estimation.
* Build interactive dashboards using Power BI or Tableau.
* Automate data ingestion from IPL datasets.

---

## 🔗 Project Link

**Google Sheets Simulation Model**

Replace the placeholder below with your shareable Google Sheets URL:

```text
[https://docs.google.com/spreadsheets/d/<YOUR_SHEET_ID>/edit](https://docs.google.com/spreadsheets/d/14cHUzhgsgPfd_qvW3Yykgd--MkVD955o/edit?usp=drivesdk&ouid=115330567433643665469&rtpof=true&sd=true)
```

---

## 📄 License

This project is intended for educational, analytical, and portfolio purposes.
