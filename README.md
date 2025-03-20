# Trust & Safety SQL Project

## Project Overview
This SQL project analyzes real-world data from the **Jigsaw Toxic Comment Classification Challenge** to support Trust & Safety operations, content moderation accuracy, and data-driven decision-making at TikTok. It specifically addresses moderation insights such as toxicity rates, trend analyses, root cause analyses, and prepares metrics for visualization.

## Data Source
**Dataset:** [Jigsaw Toxic Comment Classification (Kaggle)](https://www.kaggle.com/competitions/jigsaw-toxic-comment-classification-challenge/data)

The dataset includes real user-generated comments from Wikipedia, labeled with toxicity indicators:
- `toxic`
- `severe_toxic`
- `obscene`
- `threat`
- `insult`
- `identity_hate`

## Key Findings & Results

### Toxicity Rate Analysis
| Metric             | Count  | Percentage |
|--------------------|--------|------------|
| Total Comments     | 159,571| 100%       |
| Toxic Comments     | 15,294 | 9.59%      |
| Severe Toxicity    | 1,595  | 1.00%      |
| Obscene Comments   | 8,449  | 5.29%      |
| Threat Comments    | 478    | 0.30%      |
| Insulting Comments | 7,877  | 4.94%      |
| Identity Hate      | 1,405  | 0.88%      |

### Top Multi-label Toxicity Patterns
| Toxic | Severe Toxic | Obscene | Threat | Insult | Identity Hate | Occurrences |
|-------|--------------|---------|--------|--------|---------------|-------------|
| 1     | 0            | 1       | 0      | 1      | 0             | 1,211       |
| 1     | 0            | 1       | 0      | 0      | 0             | 1,031       |
| 1     | 0            | 0       | 0      | 1      | 0             | 734         |
| 1     | 0            | 0       | 0      | 0      | 1             | 539         |
| 1     | 1            | 1       | 0      | 1      | 0             | 367         |

**Insight:** Obscenity combined with general toxicity and insults represent the most frequent complex moderation cases.

### Monthly Toxic Comments Trend (Simulated Dates)
| Month    | Total Comments | Toxic Comments | Toxicity % |
|----------|----------------|----------------|------------|
| 2023-09  | 26,410         | 2,552          | 9.66%      |
| 2023-10  | 26,678         | 2,568          | 9.62%      |
| 2023-11  | 26,703         | 2,531          | 9.48%      |
| 2023-12  | 26,670         | 2,553          | 9.57%      |
| 2024-01  | 26,529         | 2,554          | 9.63%      |
| 2024-02  | 26,581         | 2,536          | 9.54%      |

**Insight:** Monthly moderation load and toxicity rates remain relatively consistent, allowing predictive resource allocation for moderation teams.

## Dashboard Recommendations
The following visualizations are recommended to clearly communicate insights:
- **Bar Chart:** Frequency distribution of toxic categories.
- **Line Chart:** Monthly toxicity trends.
- **Heatmap:** Visualization of common multi-label toxicity patterns.

## Skills Demonstrated
- SQL data import, cleaning, and normalization
- Advanced analytical queries (Root Cause Analysis, trends)
- Preparation of business-ready dashboards
- Effective data storytelling to support Trust & Safety operations

## Next Steps & Future Enhancements
- Integrate sentiment analysis or machine learning for predictive moderation.
- Automate pipeline processes for daily reporting.
- Expand to include user interaction metrics for holistic Trust & Safety insights.
