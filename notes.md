Key Notes:
- We are going to take the data from the reports and transform them into the "quote" object
    - We want to be able to quickly see what data represents the quote instead of searching reports
    - We may need to adjust the data to better fit next steps
    - We may get different version of the data from multiple reports and this will show how merging will be working
- Store only report lookup location and basic report data post tranlation
    - reduces the size of the overall object
    - saved by the api gateway and can be looked up there during audits
    - Audits will need raw data regardless, stored in api calls long term
- Underscores are used with lower case values
    - Consistentcy and readability with the various systems (JS, JSON, C#, Coherent, Excel)
- We won't use nested arrays
    - Coherent (excel) can't work with arrays within arrays
    - Building is flattened into Location
    - Other lists of lists need to follow a simple progression to work well within Coherent
    
