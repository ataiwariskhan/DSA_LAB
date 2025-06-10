# Blending impact on filter 
1.Add a filter from coffee chain and observe it's effect on SuperStore 
2. Identify and resolve filter behaviour mismatch using linkage logic

## Step 1: Load the Data Sources
- Open Tableau Desktop.
- Connect to the SuperStore dataset.
- Click on Data > New Data Source and connect to the Coffee Chain dataset.
- Ensure both datasets appear in the Data Pane.
## Step 2: Create a Blended View
- Open a new worksheet.
- Drag a common dimension (e.g., State or Category) from SuperStore onto the view.
- Add a measure (e.g., Sales or Profit) from SuperStore.
- Now, drag a measure from Coffee Chain (e.g., Sales or Profit).
- Tableau will automatically blend the data based on the common dimension (look for the chain icon next to the linking field)
## Step 3: Manually Enable Linkage
- Go to the Data Pane.
- Locate the common field in the secondary data source.
- Click the broken chain icon next to the field to activate the link.
- Once linked, the chain icon will turn solid, indicating that the data sources are now connected.
## Step 4: Apply Filters and Validate Linkage
- Drag a dimension from the primary data source onto the view.
- Add a measure from the secondary data source.
- Apply a filter from the primary data source and observe if it affects the secondary source.
- If the filter does not propagate, check if the linking field is correctly set.
## Step 5: Resolve Linkage Issues
- If filters do not work as expected:
- Ensure the linking field exists in both datasets.
- Verify that the values in the linking field match across both sources.
- If necessary, use parameters or LOD (Level of Detail) calculations to synchronize filtering across datasets
