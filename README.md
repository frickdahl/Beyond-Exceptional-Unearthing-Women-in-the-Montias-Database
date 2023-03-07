# Beyond-Exceptional-Unearthing-Women-in-the-Montias-Database

**The CSV Files:**

For this project, two CSV files were created containing information related to the 168 inventories in the Montias Database of 17th-Century Dutch Art Inventories (MD) dated to the 1630s. The 1630s are an optimal starting point because of the artistic and mercantile flourishing in the Dutch Republic during this decade. The incorporation of the two trading companies, the Dutch East India Company in 1602 and the Dutch West India Company in 1621, led to an influx of wealth and imported rarities, such as Chinese porcelain, spices, naturalia, and other commodities, into Amsterdam. The port city was also an essential hub for artists, artisans, collectors, and art dealers. Prominent art-historical figures who appear in the 1630s network include painter Rembrandt van Rijn (1606–1669), whose portraits were highly coveted by wealthy collectors, and ebony worker Herman Doomer (1595–1650), who created luxurious furniture pieces, often embellished with imported ebony and scintillating mother of pearl.

The first CSV file, “MD1630s_nodelist,” lists the nodes (individuals and, occasionally, institutions) and their attributes. In addition to including inventory owners, the file incorporates individuals mentioned in Montias’s commentary and buyer’s notes to add complexity to the network. Some MD inventories from outside the 1630s have been included if the inventory owner was mentioned in a 1630s inventory. Attributes include information from the inventories related to their owners, creation, and the objects they describe. A series of attributes have been prioritized based on the aims of the project. These include historical significance, marital status at the time of the inventory’s creation, sex of the inventory owner, nationality, and specific categories of objects owned. Scholars consulting the file can easily change these attributes in the code and node list CSV to suit research needs. The inventory’s purpose has been included as an attribute but simplified for efficiency.

The inventory purpose categories in the “MD1630s_nodelist” are:
- Unknown
- Death 
- Goods
    - Inventory of goods in the owner’s domain 
    - Goods left in usufruct
    - List of goods brought to the house of the inventory owner
    - Inventory of goods owned in common after the death of the spouse 
    - Court-ordered inventory (probably for an insolvent owner)
    - Goods taken in arrest pursuant to the failure to pay a debt of 279 f.
- Auction
- Prenuptial
- Execution of Court Sentence
- Inventory Drawn at Request
    - For the benefit of creditors 
    - By the request of a court officer
- Marriage
- Transfer or Sale
    - As collateral to secure a debt
- Bankruptcy
- Insolvency
- Evaluation of Inheritance
- Court Ordered
- Sale
    - Sold at the request of the owner or other parties
    - To compensate for debt
    - As collateral for a loan
- Transfer
    - As collateral for surety on a loan
    - To secure objects before extended travel
    - Goods transferred in payment for lapsed house rents

The other file, “MD1630s_edgelist,” lists the edges or connections between two individual nodes. As the network is undirected, it does not matter which individual is listed in the source or target columns.


**Python and Networkx Method:**
There are two main methods for analyzing CSV files with social-network analysis. The first and more involved method is to use Python and the NetworkX suite of Python tools. If employing this method, it is suggested that you become familiar with the basics of the ubiquitous coding language, Python. There are several free resources and inexpensive courses available online. The code utilized in this project was adapted from John R. Ladd, Jessica Otis, Christopher N. Warren, and Scott Weingart, [“Exploring and Analyzing Network Data with Python,”](https://programminghistorian.org/en/lessons/exploring-and-analyzing-network-data-with-python) Programming Historian 6 (2017). Ladd et al.’s publication is also an excellent and in-depth tutorial for using Python to create and analyze a historical social network. Additional algorithms can be found on and adapted from NetworkX’s [reference page](https://networkx.org/documentation/stable/reference/index.html). The code was modified using Juypter notebooks, but several other computing platforms are also suitable for this process. The code, made available here, can easily be altered and expanded to meet the criteria of projects depending on the researcher’s aims. Comments have been included throughout the code to assist researchers with utilizing and editing the code to fit their needs. The above-defined Python/NetworkX protocol can be combined with the following method by saving the project in the code as a graph file.


**Data Visualization Software Method:**
The other method is to apply data visualization software that does the computing for you. Several free data visualization tools are available, including some designed specifically for humanities projects, such as [Palladio](https://hdlab.stanford.edu/palladio/) (Stanford University). This project utilized Gephi 0.9.7, an open-source and free visualization and exploration software. After opening Gephi, select “Start New Project.” You can manually enter individual nodes and edges using the “Add” function under the “Data Laboratory” tab. Go to “File” for larger datasets and select “Import Spreadsheet.” You can then import your two files separately. Make sure to upload them to the appropriate “Nodes” and “Edges” sections of the “Data Laboratory” section. After importing your data, Gephi has dozens of tools to interrogate the network and allows you to design visually appealing graphs of the data. There are many helpful video tutorials available on YouTube that can assist you in this process.
