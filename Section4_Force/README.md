1. Replace the stock dataset `graph.csv` with a different one.  
I'd suggest looking at the flights dataset from lab 6, which I attached as `flights.csv.gz`.  
I picked out city pairs with more than 100 flights between them in the dataset and put them on the graph.  
When you load in the new dataset, pay attention to what the columns of `graph.csv` are called, and how they get referred to in `d3.csv()` in `index.html`.


2. The graph now looks... not great. Everything's clumped together. Change the parameters of the force diagram [(see the documentation)](https://github.com/d3/d3-3.x-api-reference/blob/master/Force-Layout.md) so that they look a bit better. Experiment with what things like `linkStrength`, `gravity`, `theta`, and what everything else do.  
Remember to use chain syntax: `d3.force().nodes(nodes).links(links).charge(-30)` etc.