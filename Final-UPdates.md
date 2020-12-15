# Final Updates

# 1. Histograms - Single Domain Pairs

**Definitions**

* **%length -** A....
* **validation_domain —**  Number of proteins-pairs with single domain in validation (provided by 3dID and pFam)
* **prediction_domain** — Number of proteins with predicted single domain (for the same above validation pairs)

## On Validation data set

For each pair we counted both the proteins even if that leads us to count some proteins more than once. This lead to total number of proteins as ~ 5000 as the number of validation pairs is ~2500

We did because in our predication of interaction-sites we might provide a different site for a protein during its interaction with another proteins. For example we might not predict the domain for P1 exactly same during PPI prediction for P1-P2 and P1-P3. Hence we will consider P1 two time (and P2 and P3 one times) for this example while comparing the domain lengths of our prediction-sites with the actual/validation domain. 

[Image: image.png]


```
**source :** dm_comparision_histogram_analysis.ipynb

plot_domin_graph_append_two_columns(single_domin_pairs_with_length, len(single_domin_pairs_with_length), '%len_A', '%len_B', 'validation_domin_pairs', 'histogram_analysis_output/single_domin_pairs_with_length.png')
```



## Algorithm wise prediction Sites on SW landscapes

### walk

[Image: image.png]

### brspot

[Image: image.png]

### Cluster-Net

[Image: image.png]

## Algorithm wise prediction Sites on Original landscapes

### walk

[Image: image.png]

### panorama

[Image: image.png]

### brspot

[Image: image.png]

### Cluster-Net

[Image: image.png]



## Comparisons : SW landscapes

### varying validation %length


[Image: image.png][Image: image.png]



## Comparisons : Original landscapes

