# AI-Recommendation-Logic-Tech-Stack-Recommender

A Python-based career recommendation system that suggests technology career paths using user skills and similarity scoring.

The project combines TF-IDF, Cosine Similarity, and Skill Coverage to generate personalized recommendations and learning guidance.

---

## Project Objective

Build a simple recommendation engine that:

- Accepts user skills
- Matches skills with career roles
- Calculates recommendation scores
- Suggests skills to learn next
- Generates visual career insights

---

## Recommendation Logic

### Formula

```text
Final Score =
0.7 × Cosine Similarity
+
0.3 × Skill Coverage
```

| Method | Purpose |
|---|---|
| TF-IDF | Gives importance to specific skills |
| Cosine Similarity | Measures skill similarity |
| Skill Coverage | Calculates matched skills percentage |

---

## Workflow

```text
User Skills
↓
Normalization
↓
TF-IDF
↓
Similarity Calculation
↓
Final Ranking
↓
Career Recommendation
↓
Graphs
```

---

## Skill Normalization

| Input | Converted To |
|---|---|
| ml | machinelearning |
| ai | artificialintelligence |
| dl | deeplearning |
| cloud | cloud aws azure |
| api | rest api |

---

## Dataset

Contains **26 technology roles** across:

| Domain | Example Roles |
|---|---|
| AI / ML | AI Engineer, ML Engineer |
| Data | Data Scientist, Data Analyst |
| Cloud | Cloud Engineer, DevOps |
| Development | Backend, Full Stack |
| Security | Cyber Security Analyst |

---

## Generated Outputs

| Output | Description |
|---|---|
| career_scores.png | Top career recommendations |
| skills_match_matrix.png | Skill matching overview |
| similarity_scores.png | Recommendation comparison |

---

## Example

### Input

```text
Python, NLP, ML, LLM
```

### Output

| Metric | Result |
|---|---|
| Recommended Role | AI Engineer |
| Match Score | 62.4% |
| Readiness | Intermediate |

### Suggested Learning Path

```text
Deep Learning
TensorFlow
PyTorch
FastAPI
Git
```

---

## Project Structure

```text
AI-Recommendation-Logic-Tech-Stack-Recommender/
│
├── recommender.py
├── raw_skills.csv
├── README.md
├── requirements.txt
└── graphs/
```

---

## Installation

```bash
pip install -r requirements.txt
```

---

## Run

```bash
python recommender.py
```

---

## Technologies

| Category | Tools |
|---|---|
| Language | Python |
| Data | Pandas, NumPy |
| ML | Scikit-learn |
| Visualization | Matplotlib, Seaborn |

---

## Learning Outcomes

- Recommendation Systems
- TF-IDF
- Cosine Similarity
- Composite Scoring
- Data Visualization

---

Future scope:
- Streamlit Web App
- Resume Recommendation
- Interactive Dashboard