# Website-Theme-A-B-Testing
This project analyzes the impact of website theme (Light vs. Dark) on user engagement and conversion metrics using A/B testing data. The analysis includes data exploration, visualization, statistical hypothesis testing, and actionable insights.

### Project Overview
This notebook investigates whether the Light or Dark website theme leads to better user engagement and conversion outcomes. The analysis uses statistical tests to compare key metrics between the two groups.

### Data Description
The dataset contains user session data from an A/B test, including:
* Theme: Light Theme or Dark Theme
* Click Through Rate
* Conversion Rate
* Bounce Rate
* Scroll_Depth
* Session_Duration
* Purchases (Yes/No)
* Added_to_Cart (Yes/No)

### Summary Statistics
| Theme           | Click Through Rate | Conversion Rate | Bounce Rate | Scroll Depth | Session Duration | Purchases | Added to Cart |
| --------------- | ------------------ | --------------- | ----------- | ------------ | ---------------- | --------- | ------------- |
| **Dark Theme**  | 0.2645             | 0.2513          | 0.5121      | 49.93        | 919.48           | 0.5039    | 0.5195        |
| **Light Theme** | 0.2471             | 0.2555          | 0.4990      | 50.74        | 930.83           | 0.5309    | 0.5329        |

### Hypotheses
* Null Hypothesis (H₀): Mean metric value is the same for Light Theme and Dark Theme.
* Alternative Hypothesis (H₁): Mean metric value differs between Light Theme and Dark Theme.

### Statistical Test Results
| Metric                 | Light Theme Mean | Dark Theme Mean | p-value | Significant? (α=0.05) |
| ---------------------- | ---------------- | --------------- | ------- | --------------------- |
| **Click Through Rate** | 0.2471           | 0.2645          | 0.0483  | ✅ Yes                 |
| **Conversion Rate**    | 0.2555           | 0.2513          | 0.6353  | ❌ No                  |
| **Bounce Rate**        | 0.4990           | 0.5121          | 0.2301  | ❌ No                  |
| **Scroll Depth**       | 50.74            | 49.93           | 0.4495  | ❌ No                  |
| **Session Duration**   | 930.83           | 919.48          | 0.7243  | ❌ No                  |

### Insights
* Click Through Rate: The difference is statistically significant (p = 0.0483), with Dark Theme achieving a higher CTR.
* All other metrics (Conversion Rate, Bounce Rate, Scroll Depth, Session Duration) show no statistically significant difference between the two themes.
### Conclusion
* The Dark Theme leads to higher engagement in terms of Click Through Rate.
* No strong evidence suggests one theme outperforms the other in conversions, bounce rate, depth, or time spent.

  In summary, while the two themes perform similarly across most metrics, the Dark Theme has a slight edge in terms of engaging users to click through. For other key performance indicators like Conversion Rate, Bounce Rate, and Scroll Depth, the choice between a Light Theme and a Dark Theme does not significantly affect user behaviour according to the data provided.


