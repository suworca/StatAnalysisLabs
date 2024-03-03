# Lab3. Visualising

## Data description
[Source: Kaggle](https://www.kaggle.com/datasets/shivam2503/diamonds)
### Context
This classic dataset contains the prices and other attributes of almost 54,000 diamonds. It's a great dataset for beginners learning to work with data analysis and visualization.
### Content 
<b>price</b> in US dollars (\$326--\$18,823)

<b>carat</b> weight of the diamond (0.2--5.01)

<b>cut</b> quality of the cut (Fair, Good, Very Good, Premium, Ideal)

<b>color</b> diamond colour, from J (worst) to D (best)

<b>clarity</b> a measurement of how clear the diamond is (I1 (worst), SI2, SI1, VS2, VS1, VVS2, VVS1, IF (best))

<b>x</b> length in mm (0--10.74)

<b>y</b> width in mm (0--58.9)

<b>z</b> depth in mm (0--31.8)

<b>depth</b> total depth percentage = z / mean(x, y) = 2 * z / (x + y) (43--79)

<b>table</b> width of top of diamond relative to widest point (43--95)
### Data Preview

|FIELD1|carat|cut      |color|clarity|depth|table|price|x    |y    |z   |
|------|-----|---------|-----|-------|-----|-----|-----|-----|-----|----|
|1     |0.23 |Ideal    |E    |SI2    |61.5 |55   |326  |3.95 |3.98 |2.43|
|2     |0.21 |Premium  |E    |SI1    |59.8 |61   |326  |3.89 |3.84 |2.31|
|3     |0.23 |Good     |E    |VS1    |56.9 |65   |327  |4.05 |4.07 |2.31|
|4     |0.29 |Premium  |I    |VS2    |62.4 |58   |334  |4.2  |4.23 |2.63|
|5     |0.31 |Good     |J    |SI2    |63.3 |58   |335  |4.34 |4.35 |2.75|
|10    |0.23 |Very Good|H    |VS1    |59.4 |61   |338  |4    |4.05 |2.39|

## Task 
1. Group the data by table, selecting 4 groups with equal intervals. Initially, clean the data from outliers using the D.Tukey method. Display it in one picture: the histogram of the distribution, polygon, cumulative.
2. Build a pie chart based on the cut attribute.
3. Build a violin chart based on price. 
4. Display a diamond scatter chart with a price above 90 percentile.

## Results
### Bar Chart
The histogram, frequency polygon, and cumulative values for the "table" characteristic (Fig. 1) indicate that the highest frequency occurs in the range of 54.575 to 57.55. This range encompasses over half of the observations and is followed by the next highest range. The third range, from 57.55 to 60.525, is also clearly visible on the histogram and has a noticeable impact on the cumulative values. The remaining ranges have significantly fewer frequencies, indicating that the majority of diamonds' "table" indicator values are concentrated in the range of 54.575 to 60.525.
### Pie Chart
The "Ideal" category is represented by the largest share and occupies the largest area on the chart. The "Premium" category comes next and also has a significant share, slightly surpassing the "Very Good" category. "Good" and "Fair" have significantly smaller shares compared to the previous categories.
### Violin Diagram
A violin graph is used to visualize the distribution of data and their probability density, in other words, the width of the sections of the diagram indicates the frequency of the indicator with a given value along the Y axis. The following features can be noted in this diagram:
* Two peaks can be clearly seen: the main one, around the value of 1000 on the price scale, and the smaller one, just below the 5000 mark. Thus, it can be concluded that the main part of the diamonds in the presented data is concentrated in the price range of about 1000, and another much smaller “cluster” can be seen just below the 5000 mark. 
* As the price increases from 5000, the number of diamonds gradually decreases
### Scatter Plot
It is clearly seen that the frequencies, depending on the color, are concentrated in certain areas of weight. Most diamonds of the E and I colors are concentrated at the 1.0 weight mark, while most of them have a price below 12,000. Also, most F and G diamonds have a weight from 1.0 to about 1.75 carats and are also concentrated at 1.5 on the horizontal axis, while those with a value less than 1.5 in carat, like E and I, mostly have a price below 12,000. The diamonds of the remaining colors are partially represented in weights from 1.5 to 2.0 carats, but for the most part they are concentrated along the horizontal axis between 2.0 and example 2.25, and as the price increases, their number also increases.