# TOPSIS-Based Model Selection for Text Generation

## Overview
This project implements the TOPSIS (Technique for Order of Preference by Similarity to Ideal Solution) method to rank pre-trained text generation models based on multiple evaluation criteria. It helps in selecting the best model by considering both beneficial and non-beneficial criteria.

## Models Evaluated
The following pre-trained models were evaluated:
- Llama-2
- Falcon
- BLOOM
- T5
- BART
- DeepSeek
- Mistral

## Evaluation Criteria
Each model was evaluated based on the following criteria:
- **Perplexity** (Lower is better)
- **BLEU Score** (Higher is better)
- **Inference Time** (Lower is better)
- **Model Size** (Lower is better)
- **Training Data Size** (Higher is better)

## Methodology
1. **Normalization**: The dataset was normalized using Min-Max scaling.
2. **Weighted Decision Matrix**: Each criterion was assigned a weight indicating its relative importance.
3. **Ideal and Anti-Ideal Solutions**: The best and worst possible values for each criterion were determined.
4. **Distance Calculation**: Euclidean distances to the ideal and anti-ideal solutions were computed.
5. **TOPSIS Score Calculation**: Models were ranked based on their relative closeness to the ideal solution.

## Dependencies
To run the project, install the required dependencies:
```bash
pip install numpy pandas matplotlib scikit-learn
```

## Output
- **Ranked List of Models**: Displays the TOPSIS scores and rankings of models.
- **Visualization**: A bar chart showcasing the rankings.

## Results Interpretation
Higher TOPSIS scores indicate better models based on the given criteria. The visualization helps in comparing different models effectively.

## Future Improvements
- Incorporate additional evaluation metrics.
- Extend the analysis to more models.
- Automate data collection from benchmarking sources.

## License
This project is open-source and available for modification and redistribution.

