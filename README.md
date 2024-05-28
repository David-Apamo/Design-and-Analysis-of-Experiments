# Design-and-Analysis-of-Experiments
This repository provides a comprehensive overview of various experimental design techniques used in scientific research and data analysis. The aim is to offer clear explanations, practical examples, and code implementations the following experimental designs:  CRD, RBD, Latin Square Design, Factorial Design and Split-plot Design. I did the analysis using R and the following R packages are required; tidyverse, agricolae and report. Please navigate to the folder with .Rmd extension, download and run the provided markdown file on your computer to see examples and analyses. I have also provided a knit file of the same for my uploaded markdown.

## Contributions
Contributions are welcome! Please open an issue or submit a pull request if you have improvements or additional examples to share.

# Contents

## 1. Completely Randomized Design (CRD)
A Completely Randomized Design (CRD) is one of the simplest experimental designs where all the experimental units are allocated randomly among the treatments.
### Characteristics
Each experimental unit is assigned to a treatment completely at random.
It is suitable when experimental units are homogeneous.
The number of replicates for each treatment can be unequal.
### Advantages
Simple to implement.
Requires minimal experimental resources.
### Disadvantages
Less efficient if there is a lot of variability among experimental units because random allocation does not account for this variability.

## 2. Randomized Block Design (RBD)
A Randomized Block Design (RBD) is used when the experimental units are heterogeneous. The units are grouped into blocks based on certain characteristics, and treatments are randomly assigned within each block.
### Characteristics
Each block contains all treatments.
Blocking reduces variability by accounting for known sources of variability.
### Advantages
More precise than CRD because it controls for the variability within blocks.
Useful when experimental units are not homogeneous.
### Disadvantages
Can be complex to implement.
Requires knowledge about the sources of variability to form appropriate blocks.

## 3. Latin Square Design
A Latin Square Design is used to control for two sources of variability. The experimental units are arranged in a square, with each row and each column representing a source of variability. Each treatment appears exactly once in each row and column.
### Characteristics
Controls for two extraneous sources of variability.
Each treatment appears once per row and once per column.
### Advantages
Efficient for controlling two sources of variability.
Reduces the number of experimental units needed compared to fully randomized designs.
### Disadvantages
May be complex to arrange.
Assumes no interaction between the two sources of variability and treatments.

## 4. Factorial Design
A Factorial Design involves studying the effects of two or more factors simultaneously. Each level of one factor is combined with each level of the other factors to create different treatment combinations.
### Characteristics
Allows for the study of interaction effects between factors.
Can handle multiple independent variables.
### Advantages
Provides comprehensive information about the main effects and interaction effects.
Efficient in terms of data collection and analysis.
### Disadvantages
Can become complex with a large number of factors or levels.
Requires a larger number of experimental units.

## 5. Split-plot Design
A Split-plot Design is used when some factors are harder to change than others. The main plot treatments (factors that are hard to change) are applied to large plots, and sub-plot treatments (factors that are easy to change) are applied within these main plots.
### Characteristics
Main plots and sub-plots allow for different levels of experimental precision.
Suitable for experiments where some factors require large-scale application.
### Advantages
Flexibility in dealing with factors that are hard or expensive to change.
Allows for the study of interactions between main plot and sub-plot treatments.
### Disadvantages
More complex analysis.
Requires careful consideration of randomization and replication.

## Note:
I used 5% as the level of significance throughout my analysis.
These designs offer various ways to structure experiments to control for different sources of variability and to study multiple factors efficiently. The choice of design depends on the specific research question, the nature of the experimental units, and practical considerations.
