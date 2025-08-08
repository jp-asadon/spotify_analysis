# 🎧 Spotify Listening Behavior Analysis

A data-driven exploration of Spotify user behavior based on detailed playback history. This project analyzes trends across time, artist and track popularity, skippability, and how listening habits changed during the COVID-19 lockdown.

---

## 📂 View Notebook

[📄 Open Visualization Notebook](https://github.com/jp-asadon/spotify_analysis/blob/main/notebook.ipynb)

---

## 📋 Table of Contents

- [About the Project](#-about-the-project)
- [Dataset](#-dataset)
- [Project Highlights](#-project-highlights)
- [Key Visualizations](#-key-visualizations)
- [How to Run](#-how-to-run)
- [Conclusion & Insights](#-conclusion--insights)
- [Future Improvements](#-future-improvements)
- [Acknowledgments](#-acknowledgments)

---

## 🧠 About the Project

This project uses Spotify listening history data to uncover insights such as:

- Which artists and songs were most played?
- Do users skip more songs when shuffle is enabled?
- How did listening behavior change during the COVID-19 pandemic?
- What playback methods (e.g., autoplay, click) result in longer listening?

---

## 📊 Dataset

**Source:** [Top Spotify Songs in Countries – Kaggle](https://www.kaggle.com/datasets/anandshaw2001/top-spotify-songs-in-countries)

**Description:**  
This dataset contains multi-year Spotify listening history of a user. Each record captures information about a track's playback metadata and user interaction.

### 📄 Data Dictionary

| Field | Description |
|-------|-------------|
| `spotify_track_uri` | Spotify URI that uniquely identifies the track |
| `ts` | Timestamp when the track stopped playing (UTC) |
| `platform` | Platform used for playback (e.g., web player, mobile) |
| `ms_played` | Milliseconds the track was played |
| `track_name` | Name of the track |
| `artist_name` | Name of the artist |
| `album_name` | Name of the album |
| `reason_start` | Why the track started (user click, autoplay, etc.) |
| `reason_end` | Why the track ended (skipped, completed, etc.) |
| `shuffle` | Whether shuffle mode was enabled |
| `skipped` | Whether the track was skipped |

---

## 📈 Project Highlights

- ✅ Data Cleaning
- ✅ Time-based Trend Analysis
- ✅ Top Artists and Tracks
- ✅ Skippability Metrics
- ✅ COVID-19 Lockdown Listening Patterns
- ✅ Playback Source & Engagement Comparison

---

## 🖼️ Key Visualizations

### 📅 Usage Trends Over Time
- Monthly/yearly track count and playback time
- Identifies the busiest listening month/day/year

### 🦠 COVID-Era Listening Behavior
- Listening trend changes with shaded bands during lockdowns
- Highlights how habits shifted in 2020–2021

### 🎤 Top Artists and Tracks
- Top 10 most played artists
- Top 10 most played tracks
- Top 10 artists with most streamed albums

### 🔁 Shuffle Mode vs. Skipping Behavior
- Measures skip frequency when shuffle is enabled
- Shows whether shuffle increases or decreases engagement

### ⏯ Playback Source vs. Duration
- Compares listening duration by start method (click, autoplay, popup, etc.)
- Pop-up driven songs tend to have longer play durations

### ✅ Unskipped Popular Songs
- Top 20 most played tracks that are least skipped
- Useful for playlist curation

### 🎯 Skippability Index
- Scatter plot of `ms_played` vs. skip rate
- Identifies which songs were enjoyed or skipped often

---

## 🚀 How to Run

### 1) Clone the repository
```bash
git clone https://github.com/jp-asadon/spotify_analysis.git
cd spotify_analysis
```

### 2) (Recommended) Create and activate a virtual environment

macOS/Linux:
```bash
python3 -m venv .venv
source .venv/bin/activate
```

Windows (PowerShell):
```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
```

### 3) Install dependencies

If a `requirements.txt` is present:
```bash
pip install -r requirements.txt
```

Or install packages directly:
```bash
pip install pandas matplotlib seaborn jupyter numpy
```

### 4) Launch Jupyter and open the notebook
```bash
jupyter notebook
```

Then open `notebook.ipynb` and run cells top-to-bottom.

> Tip: You can also use `jupyter lab` if you prefer.

---

## 📌 Conclusion & Insights

From the analysis:

- Shuffle mode increases skipping behavior — users tend to skip more songs when shuffle is ON.
- Pop-up initiated playback results in longer listening durations compared to autoplay or manual clicks.
- Certain artists and tracks consistently appear in shuffle playback and are rarely skipped, showing strong listener loyalty.
- COVID-19 lockdown periods saw significant shifts in listening habits, including an increase in total listening time and a change in top artists.

---

## 🔭 Future Improvements

- Integrate additional user-level context (e.g., mood, activity)
- Use the Spotify API to supplement metadata
- Build an interactive dashboard (e.g., Streamlit) for real-time exploration

---

## 🙌 Acknowledgments

- Dataset by [Anand Shaw](https://www.kaggle.com/anandshaw2001) on Kaggle

---


```

