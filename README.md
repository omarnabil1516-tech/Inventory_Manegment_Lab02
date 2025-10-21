Inventory Optimization: EOQ with Price Breaks
Lab 02 - Order Quantities When Demand is Approximately Level
This repository contains a Jupyter Notebook that solves the Economic Order Quantity (EOQ) problem for a product with a vendor's "all-units" quantity discount schedule. The program determines the cost-minimizing order quantity by analyzing the trade-offs between purchase costs, ordering costs, and inventory holding costs.
📝 Project Overview
The objective is to develop a robust and reusable tool for making optimal purchasing decisions under a price-break scenario. The notebook reads key business parameters, performs the necessary calculations, visualizes the cost landscape, and provides a clear recommendation. It also explores several "what-if" scenarios and advanced inventory management concepts through discussion questions and bonus challenges.
✨ Key Features
EOQ Calculation: Computes the nominal EOQ for each price tier.
Feasibility Analysis: Determines if the calculated EOQ is valid within its price tier.
Total Annual Cost (TAC) Modeling: Accurately calculates the total cost, including purchasing, ordering, and holding costs for any given order quantity.
Optimal Policy Identification: Identifies the order quantity that minimizes the total annual cost.
Data-Driven Visualization: Generates a clear plot of the cost curves, showing the price breaks and the optimal order point.
Discussion & Insights: Answers critical managerial questions regarding cost savings, sensitivity to parameters, and break-even points.
Bonus Challenges Implemented:
Incremental Discounts: Logic to handle incremental discount schedules.
Heatmap Analysis: A visual sensitivity analysis of the optimal quantity based on changing demand and carrying costs.
Reorder Point (ROP) Calculation: A function to determine when to place an order.
🛠️ Prerequisites
To run this notebook, you will need Python 3.7+ and the following libraries:
Jupyter Notebook or JupyterLab
Pandas
NumPy
Matplotlib
Seaborn
🚀 Getting Started
1. Clone the Repository (Optional)
If this were a full repository, you would clone it. For now, simply save the notebook file (.ipynb) and this README.md file in a local directory.
2. Install Dependencies
Open your terminal or command prompt and install the required Python libraries using pip:
code
Bash
pip install jupyterlab pandas numpy matplotlib seaborn
3. Run the Notebook
Navigate to the project directory in your terminal:
code
Bash
cd path/to/your/project/directory
Launch JupyterLab:
code
Bash
jupyter lab
From the JupyterLab interface in your browser, open the .ipynb file.
You can run the cells one by one or execute the entire notebook by selecting Kernel > Restart & Run All.
Notebook Structure
The Jupyter Notebook is organized into the following sections:
Setup and Data Input: Imports libraries and defines the base case parameters and discount schedule.
Core Logic: All-Units Discount Analysis: Contains the Python functions for the main EOQ algorithm.
Results and Visualization:
A. Candidates Table: A summary table of the analysis for each price tier.
B. Cost Curve Plot: The graphical representation of Total Annual Cost vs. Order Quantity.
C. Recommendation: A clear, concise recommendation of the optimal policy.
Discussion Questions: Data-driven answers to the four questions posed in the lab assignment.
Bonus Challenges: Implementation and demonstration of the three optional challenges.
📊 Example Case Parameters
The analysis is based on the following example data:
Global Parameters
Parameter	Value
Annual Demand (D)	100 units
Ordering Cost (K)	$45 per order
Carrying Rate (i)	20% per year
All-Units Discount Schedule
Min Quantity	Max Quantity	Unit Price
1	49	$120.00
50	99	$115.00
100	∞	$110.00
📈 Expected Output
Running the notebook will produce:
A pandas DataFrame summarizing the candidate order quantities and their costs.
A Matplotlib plot visualizing the distinct cost curves and the optimal (Q, TAC) point.
A final recommendation paragraph.
Calculations and answers for all discussion questions and bonus challenges.