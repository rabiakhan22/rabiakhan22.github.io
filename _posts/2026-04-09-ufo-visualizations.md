---
title: UFO Sightings Visualizations
tags: [Data Visualization, UFO]
style: fill
color: primary
description: Two visualizations of UFO sightings across the United States.
---

<div class="left">
<a class="m-1 btn btn-outline-primary btn-sm" href="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/ufo-scrubbed-geocoded-time-standardized-00.csv">
  The Data
</a>
</div>

<div class="right">
<a class="m-1 btn btn-outline-primary btn-sm" href="https://github.com/rabiakhan22/rabiakhan22.github.io/blob/main/ufo_visualizations.ipynb">
  The Analysis
</a>
</div>

## UFO Sightings by Shape

<vegachart schema-url="{{ site.baseurl }}/assets/ufo_shapes.json" style="width: 100%"></vegachart>

This visualization shows the distribution of UFO sighting shapes reported across the United States. I used a nominal encoding for UFO shape on the y-axis and a quantitative encoding for the count of sightings on the x-axis. I chose a teal color scheme where color intensity also encodes the count, reinforcing the magnitude visually. To prepare the data, I filtered the dataset to only US sightings, dropped rows with null shape values, and removed entries labeled "unknown." The chart is interactive — clicking on a bar highlights that shape and grays out the others, making it easy to focus on a specific shape.

## UFO Sightings by State

<vegachart schema-url="{{ site.baseurl }}/assets/ufo_states.json" style="width: 100%"></vegachart>

This visualization shows the top 20 US states by number of UFO sightings. I used a nominal encoding for state on the y-axis and a quantitative encoding for count on the x-axis. I chose an orange color scheme where darker colors indicate higher sighting counts, making it immediately clear which states dominate. The data was aggregated by state and limited to the top 20 to keep the chart readable.

<script src="https://cdn.jsdelivr.net/npm/vega@5"></script>
<script src="https://cdn.jsdelivr.net/npm/vega-lite@5"></script>
<script src="https://cdn.jsdelivr.net/npm/vega-embed@6"></script>