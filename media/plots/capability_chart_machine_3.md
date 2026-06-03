library(qcc)
library(htmlwidgets)
library(plotly)

# Filter data for Machine 3 at Temperature 338K and Pressure 200kPa
machine_data <- X005[X005$Machine == 3 &
                     X005$Temperature == 338 &
                     X005$Pressure == 200, ]
machine_data$PartLength <- as.numeric(machine_data$PartLength)

valid_part_length <- na.omit(machine_data$PartLength)

TARGET = 50
USL = 55
LSL = 45

capability_plot <- plot_ly(x = ~valid_part_length, type = 'histogram', histnorm = 'density', name = 'Distribution', marker = list(color = '#0072B2')) %>% 
  add_lines(x = ~c(LSL, LSL), y = ~c(0, max(hist(valid_part_length, plot = FALSE)$density)), name = 'LSL', line = list(color = '#D55E00', dash = 'solid')) %>% 
  add_lines(x = ~c(USL, USL), y = ~c(0, max(hist(valid_part_length, plot = FALSE)$density)), name = 'USL', line = list(color = '#D55E00', dash = 'solid')) %>% 
  add_lines(x = ~c(TARGET, TARGET), y = ~c(0, max(hist(valid_part_length, plot = FALSE)$density)), name = 'Target', line = list(color = '#009E73', dash = 'dot')) %>% 
  layout(title = list(text = "Process Capability Chart for PartLength (Machine 3 at 338K, 200kPa)", font = list(size = 18)),
                 xaxis = list(title = list(text = "PartLength", font = list(size = 18)), tickfont = list(size = 14)),
                 yaxis = list(title = list(text = "Density", font = list(size = 18)), tickfont = list(size = 14)),
                 plot_bgcolor = 'white', paper_bgcolor = 'white', showlegend = TRUE)

htmlwidgets::saveWidget(capability_plot, file = "media/plots/capability_chart_machine_3.html", selfcontained = TRUE)
