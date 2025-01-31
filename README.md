# Python-Day-57-Creating-interactive-visualizations-with-Plotly
This project explains about the Creating interactive visualizations with Plotly
pip install plotly
import plotly.express as px
import plotly.graph_objects as go

# Sample dataset: iris dataset (included in Plotly)
df = px.data.iris()

# Scatter plot
fig = px.scatter(df, x='sepal_width', y='sepal_length', color='species', title="Iris Dataset Scatter Plot")

# Show interactive plot
fig.show()

# Sample dataset: Gapminder dataset (included in Plotly)
df = px.data.gapminder()

# Line plot
fig = px.line(df, x='year', y='gdpPercap', color='continent', title="GDP per Capita Over Time")

# Show interactive plot
fig.show()

# Sample dataset: tips dataset (included in Plotly)
df = px.data.tips()

# Bar plot
fig = px.bar(df, x='day', y='total_bill', color='sex', title="Total Bill by Day and Gender")

# Show interactive plot
fig.show()

# Histogram
fig = px.histogram(df, x="total_bill", nbins=30, title="Histogram of Total Bill")
fig.show()
