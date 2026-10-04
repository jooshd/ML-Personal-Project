# Volleyball Analytics Projects

## 1. Time-Series & Trajectory Analysis

### Project: Serve Trajectory & Landing Spot Clustering
* **Objective:** Identify serve patterns (e.g., jump float vs. top-spin trajectory signatures) and cluster target landing zones to build tactical scouting heatmaps.
* **Tasks:**
  * Preprocess time-series spatial coordinates $(x, y, t)$ of ball trajectories.
  * Apply unsupervised clustering (DBSCAN, Gaussian Mixture Models) or Functional Data Analysis (FDA) to categorize serve trajectories and pinpoint defensive vulnerabilities.
* **Available Datasets:**
  * Synthesized trajectory vectors derived from tracking datasets (VolliQ, TrackNet) or parsed spatial coordinates in DataVolley scouting logs.

---

## 2. In-Rally Point Expectancy & Win Probability

### Project: In-Rally Point Expectancy
* **Objective:** Estimate a team's probability of winning a point given the current rally state (e.g., quality of first touch, setter location, number of available attackers).
* **Tasks:**
  * Clean and engineer temporal features from touch-by-touch play data (e.g., transition state matrices, serve rating, pass quality).
  * Train gradient boosted trees (XGBoost, LightGBM) or a Bayesian hierarchical model to compute real-time point-win probabilities after each contact.
* **Available Datasets:**
  * **DataVolley / openvolley R & Python Ecosystem:** Deep repositories of DataVolley files (`.dvw`) are publicly accessible via the `openvolley` project on GitHub. These contain stroke-by-stroke scout data (e.g., serve type, pass evaluation $0\text{--}3$ scale, attack trajectory, block positioning) for hundreds of professional matches.


---

## 3. Just Volleyball NN

### Project: Models to play Just Volleyball
* **Objective:** Models to learn and adapt to the game Just Volleyball and achieve the highest win percentage
* **Tasks:**
  * Decide on a screen based (Computer Vision) or RAM/Memory inspection (State-Based) model to read in information from the game
  * Train model to play the game optimally and win as many games as possible
  * Keep track of evolution of the models through documentation

  