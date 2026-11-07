# Bandit-Based Material Screening

Project 5, Unit 5: Real-World RL Homework Projects

## Problem statement
"A multi-armed or contextual bandit that chooses which candidate alloys or compounds to 'test' next from a public dataset (e.g., Matbench)."

## About the project
A researcher has a limited testing budget and must decide which steel to test next. We model this as a multi-armed bandit, where each steel is an arm and each test returns a noisy measurement of its yield strength (MPa).

- **Data:** 60 steels sampled from the matminer `steel_strength` dataset (experimental yield strength). The reported values are used as hidden true strengths. Measurement noise is simulated.
- **Algorithms:** Random (baseline), Epsilon-Greedy, UCB1 and Thompson Sampling.
- **Setup:** 300 tests per run, 30 independent seeds, same steels and noise for every algorithm.
- **Metrics:** cumulative reward, regret, best-steel identification and exploration versus exploitation.
- **Result:** Thompson Sampling earned the most reward and had the lowest regret. Standard UCB1 stayed close to Random at this budget.

## Files
| File | Description |
|---|---|
| `Bandit_Based_Material_Screening.ipynb` | Full implementation (Google Colab notebook) |
| `Problem_Formulation.pdf` | One-page problem formulation |
| `Results_and_Learning_Curves.pdf` | Plots and interpretation |
| `REPORT.docx` | Full project report |
| `ppt.pptx` | Five-slide presentation |
| `results.zip` | Figures and results from the executed notebook |

## How to run
1. Open `Bandit_Based_Material_Screening.ipynb` in Google Colab.
2. Click Runtime > Run all. An internet connection is needed to download the dataset.

## Team
| Name | Roll No. |
|---|---|
| Hrudya Gali | 100523729020 |
| Pujyank Komari | 100523729031 |
| Sai Nanditha Azmera| 100523729055 |
