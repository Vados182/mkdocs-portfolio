# Analiza EDA i Segmentacja Rynku Airbnb w Nowym Jorku (Python & SQL)

**2026-06-02**

Kompleksowa analiza eksploracyjna (EDA) danych o wynajmie krótkoterminowym Airbnb w Nowym Jorku (48k+ rekordów). Celem projektu było zrozumienie struktury cenowej, identyfikacja czynników wpływających na popularność ofert oraz zaawansowane wykrywanie anomalii rynkowych. W projekcie połączyłem elastyczność biblioteki Pandas z wydajnością silnika relacyjnego DuckDB (SQL), co pozwoliło na sprawne czyszczenie danych, analizę statystyczną oraz stworzenie czytelnych wizualizacji w Seaborn. Projekt dowodzi umiejętności pracy w środowisku hybrydowym (Python + SQL) oraz podejścia opartego na logice biznesowej.

<a href="airbnb.ipynb" class="md-button md-button--primary">Pobierz Notebook</a>

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
