# Rapport: Arbetsflöde för AI-projekt med Linjär Regression

## Introduktion
I moderna samhällen används maskininlärning (ML) för att förutspå komplexa samband i data. Ett typiskt exempel är förutsägelse av huspriser med hjälp av algoritmen linjär regression. I denna rapport går vi igenom de kritiska stegen i arbetsflödet för ett sådant projekt.

## Datainsamling
**Hur man samlar in datan:** Data kan samlas in genom offentliga fastighetsregister, mäklare, eller andra databaser som håller information om bostadsförsäljningar.

**Format:** Datan kan sparas i CSV, Excel, SQL-databaser eller andra lämpliga dataformat som stöds av ML-verktyg.

**Lagringsplats:** Data kan lagras lokalt, i molnet (t.ex. AWS S3, Google Cloud Storage) eller i relationsdatabaser som MySQL eller PostgreSQL.

## Datavisualisering
För att förstå datans struktur och relationer kan vi använda visualiseringsverktyg. 
- **Diagram:** Spridningsdiagram (scatter plots) för att visa relationen mellan två variabler.
- **Histogram:** För att visa fördelningen av huspriser.
- **Geografiska kartor:** Visa huspriser baserade på geografiskt läge.

Verktyg som Matplotlib, Seaborn eller Plotly i Python kan användas för detta ändamål.

## Databearbetning
Datan kan behöva rengöras, normaliseras eller transformeras.
- **Rengöring:** Ta bort eller ersätt saknade värden.
- **Normalisering:** Skala data så att alla features har samma skala, t.ex. 0 till 1.
- **Kodning:** Omvandla kategoriska data till numeriska värden med "one-hot encoding" eller liknande tekniker.

Biblioteker som Pandas eller Scikit-learn i Python är utmärkta verktyg för databehandling.

## Linjär Regression
Linjär regression är en ML-algoritm som försöker passa in en linje genom datapunkter på ett sådant sätt att avståndet (oftast kvadraten av avståndet) mellan linjen och varje datapunkt minimeras. Målet är att när en ny datapunkt (hus) introduceras, kan linjen ge en bra uppskattning av dess pris.

## Driftsättning
När modellen är tränad kan den driftsättas i en produktionsmiljö.
- **Lokal driftsättning:** Genom API:er eller inbyggda applikationer.
- **Molnbaserad driftsättning:** Plattformar som AWS SageMaker, Google AI Platform eller Azure ML kan användas.

## Teknologier i maskininlärningsprocessen
- **Datainsamling:** Web scraping-verktyg som Beautiful Soup, databaser som PostgreSQL.
- **Datavisualisering:** Matplotlib, Seaborn, Plotly.
- **Databearbetning:** Pandas, Scikit-learn.
- **Träning av modell:** Scikit-learn, TensorFlow, PyTorch.
- **Driftsättning:** AWS SageMaker, Flask (för API), Docker (för containerisering).

## Avslutning
Att bygga en ML-applikation för att förutsägelse av huspriser med linjär regression involverar flera steg från insamling av data till driftsättning. Genom att förstå och noggrant genomföra varje steg kan vi skapa en robust och effektiv modell.

### Källor: 
1. [Scikit-learn documentation](https://scikit-learn.org/)
2. [Pandas documentation](https://pandas.pydata.org/)
3. [Matplotlib documentation](https://matplotlib.org/)
