<!-- Scripts to link to the Vega/Vega-Lite runtime -->
<script src="https://cdn.jsdelivr.net/npm/vega@5"></script>
<script src="https://cdn.jsdelivr.net/npm/vega-lite@4"></script>
<script src="https://cdn.jsdelivr.net/npm/vega-embed@6"></script>

# Public Bicycle Use Across London

How can we understand and compare patterns of human movement? Are individuals moving more or less than normal at the moment? And where in London are people moving?

We estimate one form of active travel – use of the [TfL Santander public bicycle hire scheme](https://tfl.gov.uk/modes/cycling/santander-cycles) – by looking at how numbers of bicycles at docking stations change every 10 minutes. By combining measures of docking station activity into localities around London we can estimate where and when travel by hire bicycle occurs (see [data processing of TfL docking stations](./dataProcessing) for more details).

By comparing daily use with that expected between January 6th and March 1st 2020 ("anomaly" calculated with the [signed chi score](https://openaccess.city.ac.uk/id/eprint/537/1/wood_visualization_2010.pdf)), we can begin to see the effect of the Covid-19 crisis on movement patterns – where and when we see more or less bicycle activity than expected. Expected use is calculated by day of week for each local region so we can account for expected weekday/weekend fluctuations.

## Visualizations

We can compare movement in local regions: through mouseover the values for an individual day, the expected value and the anomaly are shown. With a mouse click on a cell, a single locality can be selected and is highlighted in all three visualisations. Shift-click allows selection of multiple localities, and double-click selects all of London.

Stations are sorted vertically by the overall volume of activity with busier areas towards the top.

<div class="wide" id="visLinkedBicycle"></div>

The vertical patterns in the charts show clearly how mobility in London after the lockdown changed and that weekday and weekend changes differ. We also see the effect of weather on, what is in many cases, discretionary travel. Not all regions in London show similar behaviour, for example regions associated with likely leisure activity (often near parks) have seen an increase in use.

## Team

Conceived and implemented by

- _[Ross Purves](https://twitter.com/GCUZH) – [Department of Geography, University of Zurich](https://www.geo.uzh.ch/~rsp/)_
- _[Ralph Straumann](https://twitter.com/rastrau) – [EBP, Data Science Team, Zurich](https://www.ebp.ch)_
- _[Jo Wood](https://twitter.com/jwolondon) – [giCentre, City, University of London](https://www.gicentre.net/jwo)_

<!-- Script containing the vis specs used above. Must be at end of document. -->
<script src="js/londonVisSpecs.js"></script>
