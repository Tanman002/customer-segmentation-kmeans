Customer Segmentation using K-Means Clustering

Overview

This project segments mall customers into five distinct groups using K-Means clustering, an unsupervised machine learning technique. By understanding customer segments based on age, income, and spending behavior, businesses can tailor their marketing strategies and improve customer engagement.

The Dataset

I worked with 200 mall customers and their data across five features: Customer ID, Gender, Age, Annual Income (in thousands), and Spending Score (1-100, assigned by the mall based on customer behavior).

What I Did

I started by exploring the data to understand what we were working with. Then I scaled the features so that income and spending would be weighted equally in the clustering algorithm. I used the Elbow Method to determine the optimal number of clusters—the graph showed a clear bend at K=5, meaning five segments made the most sense.

I trained the K-Means model and assigned each customer to one of these five groups. Finally, I analyzed what each segment actually meant by looking at their average age, income, and spending patterns, and I translated these numbers into real business strategies.

The Five Customer Segments

Enthusiasts (Average age 33, Income $87k, Spending 82/100) These are your best customers right now. They have money and they love shopping. Strategy: Keep them loyal with rewards programs and exclusive offers.

Wise Ones (Average age 43, Income $55k, Spending 50/100) These customers have a solid budget but are selective about what they buy. They want to see more options. Strategy: Send them WhatsApp updates and direct emails showcasing new products.

Ambitious Youth (Average age 25, Income $26k, Spending 79/100) Young people with modest incomes who spend a high proportion of what they earn. They're enthusiastic shoppers. Strategy: Offer them promos, discounts, and value bundles to keep them coming back.

Busy Bees (Average age 41, Income $88k, Spending 17/100) This is the most interesting segment. They earn the highest income but spend the least at the mall. This suggests they're constrained by time, not money. Strategy: Introduce home delivery and online shopping options to capture this untapped revenue.

Value Seekers (Average age 45, Income $26k, Spending 21/100) Budget-conscious shoppers who don't have much to spend. Strategy: Focus on driving footfall with big sales events like End of Season Sale and clearance events.

Key Insight

The Busy Bees segment represents our biggest revenue opportunity. These are high earners ($88k average) who currently spend the least ($17 out of 100). The data suggests this isn't a budget problem—it's likely a time problem. If we can make shopping easier for them through delivery or online options, we could unlock significant additional revenue.

How to Use This

Open the notebook file in Google Colab (easiest option) or run it locally with Jupyter. The notebook walks through every step: data exploration, scaling, choosing the number of clusters, training the model, and interpreting the results.

If you're running it locally, install the required libraries first:

pip install pandas numpy matplotlib seaborn scikit-learn

Then open Jupyter and run the notebook.

What's Inside This Folder

The notebook contains all the code and analysis. The data folder has the customer dataset as a CSV file. The images folder contains the scatter plot showing how the five segments are distributed across income and spending.

Technologies I Used

Python, Pandas for data handling, Scikit-Learn for the K-Means algorithm, Matplotlib and Seaborn for visualization, and NumPy for numerical operations.

What I Learned

How K-Means clustering works and why feature scaling is critical
How to interpret unsupervised learning results in business terms
The importance of choosing K thoughtfully (elbow method) rather than arbitrarily
How to communicate data insights to non-technical stakeholders
I learned how unsupervised learning works—how the model finds patterns without being told what to look for. I learned why scaling features matters for distance-based algorithms like K-Means. Most importantly, I learned that the real value of clustering isn't just the clusters themselves, but the business decisions you can make from understanding what each cluster means.

Future Improvements

Experiment with other clustering algorithms (Hierarchical Clustering, DBSCAN)
Add more features (e.g., purchase frequency, product categories) for richer segmentation
Test on a messier, real-world e-commerce dataset
Build an interactive dashboard to explore segments dynamically

Next Steps

I'd like to test this approach on a messier, real-world e-commerce dataset to see if the same segments emerge. I'm also curious to try other clustering algorithms like Hierarchical Clustering or DBSCAN to compare results. Eventually, building an interactive dashboard where someone could explore these segments dynamically would be valuable.

contact
If you have questions about this project, feel free to reach out via GitHub or email.
