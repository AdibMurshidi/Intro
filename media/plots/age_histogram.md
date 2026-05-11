
```R
# Load required libraries
library(plotly)
library(htmlwidgets)

# Create the histogram
plot_ly(data = bigclass, x = ~age, type = "histogram",
        marker = list(color = "#0072B2")) %>%
  layout(title = list(text = "Age Distribution in BigClass Dataset", font = list(size = 18)),
         xaxis = list(title = "Age", titlefont = list(size = 18), tickfont = list(size = 14), zeroline = FALSE),
         yaxis = list(title = "Frequency", titlefont = list(size = 18), tickfont = list(size = 14), zeroline = FALSE),
         plot_bgcolor = "#ffffff",
         paper_bgcolor = "#ffffff") -> p

# Save the plot as an HTML widget
saveWidget(p, file = "media/plots/age_histogram.html", selfcontained = TRUE)
```
