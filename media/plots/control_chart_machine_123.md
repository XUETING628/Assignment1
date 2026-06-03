library(qcc)
library(htmlwidgets)
library(plotly)

# Filter data for Machine 1, 2, 3 at Temperature 338K and Pressure 200kPa
machine_data <- X005[X005$Machine %in% c(1, 2, 3) &
                     X005$Temperature == 338 &
                     X005$Pressure == 200, ]
machine_data$PartLength <- as.numeric(machine_data$PartLength)

valid_part_length <- na.omit(machine_data$PartLength)

control_chart_obj <- qcc(valid_part_length, type="xbar.one", nsigmas=3, plot=FALSE)

center_line <- control_chart_obj$center
lcl <- control_chart_obj$limits[1]
ucl <- control_chart_obj$limits[2]
plot_index <- 1:length(valid_part_length)

control_chart_plot <- plot_ly(x = ~plot_index, y = ~valid_part_length, type = 'scatter', mode = 'lines+markers', name = 'PartLength') %>% 
  add_trace(y = ~rep(center_line, length(plot_index)), mode = 'lines', name = 'Center Line', line = list(color = '#0072B2', dash = 'dash')) %>% 
  add_trace(y = ~rep(ucl, length(plot_index)), mode = 'lines', name = 'UCL', line = list(color = '#D55E00', dash = 'dash')) %>% 
  add_trace(y = ~rep(lcl, length(plot_index)), mode = 'lines', name = 'LCL', line = list(color = '#D55E00', dash = 'dash')) %>% 
  layout(title = list(text = "Control Chart for PartLength (Machine 1,2,3 at 338K, 200kPa)", font = list(size = 18)),
                 xaxis = list(title = list(text = "Observation", font = list(size = 18)), tickfont = list(size = 14)),
                 yaxis = list(title = list(text = "PartLength", font = list(size = 18)), tickfont = list(size = 14)),
                 plot_bgcolor = 'white', paper_bgcolor = 'white', showlegend = TRUE)

htmlwidgets::saveWidget(control_chart_plot, file = "media/plots/control_chart_machine_123.html", selfcontained = TRUE)
