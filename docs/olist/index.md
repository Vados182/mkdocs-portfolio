# Analiza EDA i Segmentacja Klientów RFM na Rynku E-Commerce (Olist & SQL)

**2026-06-19**

Kompleksowa analiza eksploracyjna (EDA) oraz zaawansowana segmentacja klientów brazylijskiego rynku e-commerce na podstawie rzeczywistych danych platformy **Olist** (ponad 100k zamówień). 

W projekcie połączyłem wydajność nowoczesnego silnika relacyjnego **DuckDB (SQL)** pracującego w pamięci z możliwościami wizualizacyjnymi bibliotek **Python (Seaborn & Matplotlib)**. Głównym celem było zbadanie integralności referencyjnej danych, identyfikacja wąskich gardeł w operacjach logistycznych oraz przeanalizowanie ich bezpośredniego wpływu na satysfakcję i oceny konsumentów. 

Zwieńczeniem analizy jest autorski model segmentacyjny **RFM (Recency, Frequency, Monetary)** zaimplementowany w czystym SQL, który dzieli bazę klientów na strategiczne grupy biznesowe (m.in. *Champions*, *Loyal Customers*, *At Risk*), umożliwiając dopasowanie spersonalizowanych działań marketingowych. Projekt doskonale demonstruje podejście zorientowane na cele biznesowe oraz umiejętność zaawansowanego modelowania danych przy użyciu SQL i Pythona.

<a href="Analiza_Olist_EDA.ipynb" class="md-button md-button--primary">Pobierz Notebook</a>

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