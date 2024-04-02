---
name: HW8 Jekyll & Vega Lite Webpage Project
tools: [Python, HTML, vega-lite]
image: assets/pngs/cars.png
description: This is a homework project that uses vega-lite for interactive viz!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Exploring Licensing Trends: An Insightful Analysis Through Visualizations

## Introduction

In this paper, we present an in-depth analysis of licensing data for the fall of 2022 using visualization techniques. We aim to reveal trends in license issuance, activation status, and modifications over time. The analysis in this paper utilizes a combination of Python, Altair, and Vega-lite. By producing visual representations and providing an interactive experience, we hope that viewers will gain insight into licensing.

## Visualization 1: License Type Distribution by Status

The first visualization offers a comprehensive view of the distribution of different license types by their status—be it active, inactive, or not renewed. This stacked bar chart elucidates the proportion of statuses within each license type, providing a clear picture of licensing dynamics across various professions.

### Analysis and Design Choices

I employed a stacked bar chart to visually segment each license type by status. The choice of vibrant, distinct colors for each status enhances readability and allows for quick comparative analysis. This visualization helps stakeholders identify areas where license renewal efforts might be intensified or better understand the landscape of professional certification.

**Interactivity Feature**: Hovering over segments of the bar reveals precise counts of licenses per status, offering an additional layer of detail to the analysis.

<vegachart schema-url="{{ site.baseurl }}/assets/json/license_type.json" style="width: 100%"></vegachart>

## Visualization 2: Trends in License Issuances Over Time

The second visualization focuses on the dynamic aspect of the licensing data—tracking how license issuances and modifications have trended over time. A line chart with markers at each point paints a vivid picture of the ebb and flow of licensure activity from month to month.

### Analysis and Design Choices

By aggregating the data monthly and plotting it over time, we discern patterns that could indicate seasonal variations in licensing activity or responses to legislative changes. The line chart was chosen for its clarity in depicting trends and the ease with which viewers can trace changes over periods.

**Enhanced Interactivity**: Beyond basic zoom and pan functionalities, this visualization incorporates a selection tool, allowing users to focus on specific time windows and probe into periods of interest by simply dragging across the timeline.

<vegachart schema-url="{{ site.baseurl }}/assets/json/license_time.json" style="width: 100%"></vegachart>

## Data Transformation and Insights
Our analysis began with data cleaning, ensuring accuracy in datetime parsing and handling missing values adeptly. The transformation phase involved aggregating licensure data to meaningful timeframes and categorizations, facilitating profound observations on trends and distribution patterns.

## Conclusion
The insights derived from these visualizations spotlight the intricacies of professional licensing, from the predominance of certain license types and statuses to discernible temporal trends in licensure activities. These analyses not only inform stakeholders but also pave the way for targeted policies and strategies in professional regulation and support.

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/vega/vega/blob/main/docs/data/cars.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/jnaiman/online_cv_public/blob/main/python_notebooks/test_generate_plots.ipynb" text="The Analysis" %}
</div>

