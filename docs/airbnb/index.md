# New York Airbnb Market Analysis

**2026-06-02**

Comprehensive exploratory data analysis (EDA) of New York City Airbnb short-term rental data (48k+ records). The project aimed to understand the pricing structure, identify factors driving listing popularity, and perform advanced market anomaly detection. I combined the flexibility of the Pandas library with the performance of the DuckDB SQL relational engine, enabling efficient data cleaning, statistical analysis, and clear visualizations using Seaborn. This project demonstrates proficiency in a hybrid environment (Python + SQL) and a business logic-driven approach. The project was written in Polish.

<a href="airbnb.ipynb" class="md-button md-button--primary">Download Notebook</a>

<iframe
    id="content"
    src="airbnb.html"
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
window.addEventListener('resize', function() {
    var iframe = document.getElementById('content');
    resizeIframeToFitContent(iframe);
});
</script>
