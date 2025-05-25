# ggDoE: An R Package for Experimental Design with an Application to Prostate Cancer Drugs

### **1. Introduction**

Experimental design plays a crucial role in scientific research, particularly in identifying how various treatments or conditions affect outcomes. In the field of cancer treatment, optimizing drug combinations to minimize cancer cell survival is a critical challenge. This project focuses on a two-level full factorial design, a statistical method used to evaluate all possible combinations of variables (factors) at two levels (e.g., low and high dosage).

To support this analysis, we explored **ggDoE**—a newly developed R package that enhances the visualization of factorial designs. ggDoE serves as a modern update to traditional experimental design tools in R, allowing researchers to better interpret and communicate complex interaction effects between factors.



### **2. Objectives**

The main goals of this research were:

* To demonstrate the use of the **ggDoE** R package in visualizing and analyzing factorial designs.
* To apply this tool to a real-world dataset involving five anti-cancer drugs used to treat prostate cancer, focusing on minimizing cancer cell survival.
* To create an R Vignette with RMarkdown that illustrates ggDoE’s functionality using the prostate cancer dataset as a case study.



### **3. Methods**

To accomplish these objectives, I used ggDoE's suite of visualization and analysis tools, including:

* `main_effect()`: Plots the average effect of a single factor.
* `interaction_effect()`: Analyzes the relationship between two interacting factors.
* `diagnostic_plots()`: Provides regression diagnostic plots.
* `halfnormal_plot()` and `pareto_plot()`: Determine which factors are statistically significant in influencing the response.

Additionally, an R Vignette was created as a practical guide for implementing ggDoE with code and visualizations, showcasing how factorial experiments can be clearly interpreted using modern data visualization techniques.



### **4. Full Factorial Design Application**

Using a dataset from Jia et al. (2017), I implemented a two-level full factorial design (2⁵ = 32 combinations) to evaluate five prostate cancer drugs (denoted D1 through D5). Each combination represents a unique presence/absence pattern of the five drugs and their effect on the survival percentage of prostate cancer cells.

The dataset was input into R, and the factorial combinations were analyzed for both main effects and interactions to determine their impact on cancer cell viability.



### **5. Results**

The factorial analysis revealed the following insights:

* **Main Effects**: D1 and D2 showed significant negative effects on cancer cell survival, indicating higher efficacy.
* **Interaction Effects**: Notable two-factor interactions included D1\:D2 and D1\:D3, suggesting that certain combinations of drugs are more effective than individual treatments.
* **Visualizations**:

  * The **Pareto plot** displayed the absolute values of all effects, helping identify the most impactful variables.
  * The **Half-normal plot** corroborated the results, visually separating significant effects from the noise.
  * **Main effect and interaction plots** provided visual summaries of how individual drugs and their pairwise combinations influenced cancer survival.

A linear model was fitted including five main effects, ten two-factor interactions, and ten three-factor interactions. Statistical significance was assessed using standard error, t-values, and p-values.



### **6. Conclusion**

This project demonstrates the power and utility of the ggDoE package in exploring complex experimental designs. The prostate cancer case study provided compelling evidence that certain drugs (notably D1 and D2) and their interactions are especially effective in reducing cancer cell survival.

By combining statistical rigor with intuitive visualizations, ggDoE enhances the transparency and accessibility of factorial analysis. The successful application to a real-world biomedical dataset underscores ggDoE’s value as a research tool for experimental design in scientific studies. As the package continues development, it promises to be a key asset for researchers aiming to optimize multi-factor experiments efficiently.

![png](poster)

