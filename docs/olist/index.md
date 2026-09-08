# EDA and RFM Customer Segmentation in E-Commerce (Olist & SQL)

**2026-06-19**

Comprehensive exploratory data analysis (EDA) and advanced customer segmentation for the Brazilian e-commerce market based on real data from the **Olist** platform (over 100k orders). 

In this project, I combined the performance of a modern in-memory relational engine **DuckDB (SQL)** with the visualization capabilities of **Python (Seaborn & Matplotlib)** libraries. The main goal was to examine data referential integrity, identify bottlenecks in logistics operations, and analyze their direct impact on consumer satisfaction and ratings. 

The culmination of the analysis is a custom **RFM (Recency, Frequency, Monetary)** segmentation model implemented in pure SQL, which divides the customer base into strategic business groups (e.g., *Champions*, *Loyal Customers*, *At Risk*), enabling tailored marketing actions. The project perfectly demonstrates a business-oriented approach and advanced data modeling skills using SQL and Python. The project was written in Polish.

<a href="Analiza_Olist_EDA.ipynb" class="md-button md-button--primary">Download Notebook</a>

<iframe
    id="content"
    src="Analiza_Olist_EDA.html"
    width="100%"
    style="border:1px solid black;overflow:hidden;"
></iframe>

<script>
function resizeIframeToFitContent(iframe) {
    iframe.style.height = (iframe.contentWindow.document.documentElement.scrollHeight + 50) + "px";
    iframe.contentDocument.body.style["overflow"] = 'hidden';
}
window.addEventListener('load', function() {
    var iframe = document.getElementById('content');
    resizeIframeToFitContent(iframe);
});
</script>