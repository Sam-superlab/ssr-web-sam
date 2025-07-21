---
{"dg-publish":true,"permalink":"/Academic/Statistics/Visualizing and Describing Data/"}
---

## Outline
- use appropriate graphs to display and describe quantitative and categorical data
- describe the **[[Academic/Statistics/distribution\|distribution]]** of a variable
- make graphs that describe the relationship between 2 or more variables

>Data Visualization displaying data in ways that make patterns more noticeable

### Data Visualization Guide Table

| Graph Type            | Variables                      | Purpose                                                                   | Pros                                        | Cons                                                        |
| --------------------- | ------------------------------ | ------------------------------------------------------------------------- | ------------------------------------------- | ----------------------------------------------------------- |
| Bar Graph             | 1 categorical                  | Display **frequency**/counts of categories                                | Simple, intuitive for comparing groups      | Limited to counts; hides distribution details               |
| Histogram             | 1 quantitative                 | Show **distribution** shape, center, spread, outliers                     | Reveals patterns (skew, modes)              | Bin size choice affects interpretation                      |
| Boxplot               | 1 quantitative                 | Summarize **center** ([[Academic/Statistics/median\|median]]), **spread** ([[Academic/Statistics/IQR\|IQR]]), and **outliers** | Robust to outliers; compact visualization   | Hides multimodality; less detail than histograms            |
| Stacked/Dodged Bar    | 2 categorical                  | Compare **proportions**/**counts** across categories                      | Shows subgroup breakdowns                   | Stacked: Hard to compare subgroups; Dodged: Space-intensive |
| [[Academic/Statistics/Scatterplot\|Scatterplot]]       | 2 quantitative                 | Explore **relationships** (form, direction, strength)                     | Reveals trends, clusters, outliers          | Overplotting with large datasets                            |
| Side-by-Side Boxplots | 1 quantitative + 1 categorical | **Compare** **distributions** across categories                           | Highlights differences in medians/IQR       | Simplifies distribution details                             |
| Faceted/Colored Plot  | 3+ variables (mix of types)    | **Multivariate analysis** (e.g., relationships across subgroups)          | Incorporates multiple variables in one plot | Complexity; may become cluttered                            |

## Association
>When there seems to be some connection between two variables (knowing about one variable tells us about the other), we say they are **associated**.

>If there does not seem to be a relationship between the variables, we say they are **independent**.
