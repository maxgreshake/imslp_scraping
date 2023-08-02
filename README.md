# imslp_scraping
python scripts for scraping data from IMSLP

Mithilfe des Skripts 'imslp_scraping.ipynb' lassen sich die HTML-Inhalte von IMSLP scrapen und die Informationen im Feld "As Dedicatee" herausfiltern. Auf diesem Wege können für die  entsprechenden Widmungsträger die jeweiligen Komponisten eruiert werden, die Werke dediziert haben. 

Für das Vorgehen sind gibt es fünf Funktionen:
1. Dedication-scraping Funktion:
Hiermit werden die HTML-Inhalte gescraped und in einer csv gespeichert. Als Argument wird die entsprechende IMSLP-URL benötigt

2. Dedication-list Funktion:
Hiermit werden die ausgegebenen CSV-Dateien zusammengefügt und die entsprechende IMSLP-URL ergänzt. Als Argument wird der Ordner, der die CSV-Dateien enthält benötigt

3. Zusatz-Scraping Funktion
Hiermit können mehrere IMSLP-Einträge, also Komponisten, zusammen gescraped werden. Als Argument wird eine Dedications-Liste benötigt

4. Nodes-List Funktion
Hiermit werden für die entsprechenden Widmungsempfänger bzw. Widmungsgeber IDs vergeben, um sie in Gephi als Nodes-Liste weiterzuverarbeiten. Als Argument wird eine Dedications-Liste benötigt

5. Edges-List Funktion
Hiermit werden die IDs aus der Node-Liste auf die Dedications-Liste übertragen, um sie in Gephi als Edges-Liste weiterzuverarbeiten. Als Argument wird eine Nodes-Liste und die entsprechende Dedications-Liste benötigt

Mit den Nodes- und Edges-Listen können weitere Analysen (RStudio) und Visualisierungen (Gephi) vorgenommen werden 
