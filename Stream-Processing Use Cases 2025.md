- Real time recommendationn for outdoor activities
- Heatwave Alerts 
- Real-time Severe Weather Alerts
- Wind Pattern tracking for aviation  
- Agricurtural support by analyzing rainfall  
 - Climate Monitoring  
- Energy demand based on heat  
- Windtracking  
- Cold hail detection

- Sichtbarkeit: Erkennt schlechte Sichtverhältnisse (z.B. unter 1000 Meter).
- Qualitätskontrolle der Stationsdaten: Meldet fehlerhafte oder verdächtige Messwerte.
- Durchschnittstemperatur-Berechnung: Gleitenden Durchschnitt der Temperatur.
- Geografischer Filter: Filtert Wetterdaten aus einer bestimmten Region.
- Zählung von Himmelsbedingungen: Zählt, wie oft bestimmte Himmelsbedingungen (z.B. 'bewölkt') auftreten.
- Plötzlicher Temperaturabfall: Meldet abrupte Temperaturabfälle (z.B. mehr als 5°C in einer Stunde).
- Sichtbarkeits-Trend verfolgen: Verfolgt, wie sich die Sichtweite über die Zeit verändert.
- Taupunktdifferenz überwachen: Berechnet die Differenz zwischen Lufttemperatur und Taupunkt (für Luftfeuchteanzeige).
- Überprüfung auf fehlende Daten: Meldet, wenn wichtige Felder regelmäßig fehlen (z.B. Temperatur oder Wind).
- Wetter-Zusammenfassung pro Station: Erstellt stündliche/tägliche Berichte mit Extremwerten und Summen je Station.

- Höchste Temperaturen in der Zeitaufteilung 0-4h 4-8h 8-12h 12-16h 16-20h 20-0h, mit Wetter Typ für jede Wetter Station
    Zweck: Wie haben sich die Klimas, im laufe der Zeit auf bezug der Höchsttemperaturen geändert. (interesstand für Klima statistiken)
- Regenfall für Monatliche/Tägliche cummalativer Wert per Region/Wetter Station
    Zweck: Wichtig für Bodeninformationen, vorallem für landwirtschaft
- Lesen von Visibilty-Obervation
    Zweck: Welche Gebiete habe viel Nebel/wenig Sichtbarkeit um Mögliche Gefahrenzonen für Verkehr und Aktivitäten zu erkennen.
- Auslesen für Luftfeuchtigkeit und Regenfall und Temperatur, pro Region
    Zweck: Erkenn welche Gebiete von Dürre (wichtig für Landwirtschaft) betroffen sind, aber auch welche Gebiete wegen Waldbrand öfters untersucht werden sollen (Hohe Temperatuzr und Trocken)
- Quality-Code Prüfen von Wind, SkyCondition, Visibility, Temperature ... (TBD)
    Zweck: Welche Wetter Daten sind Fehleranfälliger, Wo könnte besser investiert warden für weniger Fehler in den Daten
- Detektion von Temperaturstürzen (Temperaturdifferenz > X °C innerhalb von 1 Stunde)
    Zweck: Frühwarnsysteme für Frostgefahr.
- Analyse von Sturm- und Hagelereignissen (Windgeschwindigkeit, Wettertyp)
    Zweck: Risikoanalyse für Infrastruktur, Versicherungen und Krisenmanagement (z. B. zur Einschätzung von Schadenwahrscheinlichkeiten)
- Live-Berechnung der gefühlten Temperatur pro Region (Temperatur- und Luftfeuchtigkeitswerte)
    Zweck: Erkennen von Hitzewellen in Echtzeit
- Analyse von Luftdruckveränderungen in Kombination mit Temperatur/Winddaten
    Zweck: Erkennung potenzieller Wetterfronten – nützlich für Wettervorhersagen und Notfallplanung
- Korrelieren von UV-Indexdaten mit Bewölkung und Wettertyp
    Zweck: Warnsystem für erhöhte UV-Strahlung, auch bei scheinbar „bedecktem Himmel“

- Erkennung von und Warnung vor Extremwetterlagen
- Live-Wetterkarte mit Darstellung aktueller Messwerte
- Erkennung fehlerhafter und/oder manipulierter Sensordaten
- Kontinuierliche Darstellung der Sensor-Messwerte in einem Dashboard
- Live-Reporting von Wetterdaten in bestimmtem Zeitintervall (z. B. Radio Ö3) oder Wetter-Apps
- Vorhersagen treffen basierend auf den letzten 1 oder mehr (2,3,4?) Wetterdaten (ML oder gleitender Mittelwert)
- Datenaufbereitung für Feuerwehr - Waldbrandgefahr (Temperatur, Wind, Niederschlagsverlauf)
- Datenaufbereitung zur Neuschneeentwicklung (Niederschlag, Temperatur)
- Datenaufbereitung für Paragleiter (Wind, Luftdruck)
- Hitze- oder Kälteperioden erkennen (ab x Tagen)
- Wettervorhersage (anhand der letzten x Tage für die nächsten y Tage - update nach z Tagen)

- Flugverkehr Optimierung (Anpassung von Flugrouten anhand Wetterdaten)
- Erkennung von Waldbrandrisiken (Kombination von Temperatur, Wind, Luftfeuchtigkeit zur Risikoabschätzung)
- Analyse von Temperatur und Feuchtigkeit zur Vorhersage von Mückenplagen oder Pollenflug
- Feinstaubbelastungserkennung 
- Schulungsdaten für Student*Innen, die Stream-Processing verstehen wollen
- Frühwarnsysteme für Unwetter (z. B. Gewitter in 2 Tagen)
- UV-Belastung (Schutz für unsere schöne Haut)
- Routenplanung (Echtzeit Warnung wegen z. B. Sturm)
- Nebelwarnung (vor allem für Abendverkehr)
- Blitzeis-Warnung (für Auto- und Flugverkehr)
- Wind und Thermik (Druck) Infos für Gleitschirm- und Fallschirmspringer

## Pattern: Summary Statistics over Interval

> Calculate basic summary statistics (min, max, count, average) over a given time interval.

**Examples:**

* An welcher Station war der Wind in den letzten 10 Jahren am Stärksten?
  -> max over the interval [now - 10 years, now]

**Use Cases**:

- Wind Pattern tracking for aviation  
- Agricurtural support by analyzing rainfall  
- Climate Monitoring  
- Windtracking  
- Taupunktdifferenz überwachen: Berechnet die Differenz zwischen Lufttemperatur und Taupunkt (für Luftfeuchteanzeige).  
- Wetter-Zusammenfassung pro Station: Erstellt stündliche/tägliche Berichte mit Extremwerten und Summen je Station.  
- Regenfall für Monatliche/Tägliche cummalativer Wert per Region/Wetter Station  
  **Zweck:** Wichtig für Bodeninformationen, vorallem für landwirtschaft  
- Auslesen für Luftfeuchtigkeit und Regenfall und Temperatur, pro Region  
  **Zweck:** Erkenn welche Gebiete von Dürre (wichtig für Landwirtschaft) betroffen sind, aber auch welche Gebiete wegen Waldbrand öfters untersucht werden sollen (Hohe Temperatur und Trocken)  
- Analyse von Sturm- und Hagelereignissen (Windgeschwindigkeit, Wettertyp)  
  **Zweck:** Risikoanalyse für Infrastruktur, Versicherungen und Krisenmanagement (z. B. zur Einschätzung von Schadenwahrscheinlichkeiten)  
- Analyse von Luftdruckveränderungen in Kombination mit Temperatur/Winddaten  
  **Zweck:** Erkennung potenzieller Wetterfronten – nützlich für Wettervorhersagen und Notfallplanung  
- Live-Wetterkarte mit Darstellung aktueller Messwerte  
- Kontinuierliche Darstellung der Sensor-Messwerte in einem Dashboard  
- Datenaufbereitung für Feuerwehr - Waldbrandgefahr (Temperatur, Wind, Niederschlagsverlauf)  
- Datenaufbereitung zur Neuschneeentwicklung (Niederschlag, Temperatur)  
- Routenplanung (Echtzeit Warnung wegen z. B. Sturm)  
- Wind und Thermik (Druck) Infos für Gleitschirm- und Fallschirmspringer

## Pattern: Predicate Based Count

> Count the number of times a predicate evaluates to true/false over a given time interval.

**Examples:**

* Anzahl Tage Temp > zb. 30°?
  -> count P(a) = True over a time interval [t_start, t_end]

**Use Cases:**

- Sichtbarkeit: Erkennt schlechte Sichtverhältnisse (z.B. unter 1000 Meter).  
- Qualitätskontrolle der Stationsdaten: Meldet fehlerhafte oder verdächtige Messwerte.  
- Zählung von Himmelsbedingungen: Zählt, wie oft bestimmte Himmelsbedingungen (z.B. 'bewölkt') auftreten.  
- Überprüfung auf fehlende Daten: Meldet, wenn wichtige Felder regelmäßig fehlen (z.B. Temperatur oder Wind).  
- Quality-Code Prüfen von Wind, SkyCondition, Visibility, Temperature ...  
  **Zweck:** Welche Wetter Daten sind Fehleranfälliger, Wo könnte besser investiert warden für weniger Fehler in den Daten  
- Korrelieren von UV-Indexdaten mit Bewölkung und Wettertyp  
  **Zweck:** Warnsystem für erhöhte UV-Strahlung, auch bei scheinbar „bedecktem Himmel“  

## Pattern:  Summary Statistics on time dependent functions over Interval

> Calculate basic summary statistics (min, max, count, average) on values derived by functions that need multiple time shifted arguments over a given time interval.

**Examples:**

* An welcher Station war die Temperatur Steigung am steilsten in den letzten Jahren?
  -> max over a time interval [t_start, t_end] of a function f(x_t, x_(t-1))

**Use Cases:**

- Plötzlicher Temperaturabfall: Meldet abrupte Temperaturabfälle (z.B. mehr als 5°C in einer Stunde).  
- Sichtbarkeits-Trend verfolgen: Verfolgt, wie sich die Sichtweite über die Zeit verändert.  
- Detektion von Temperaturstürzen (Temperaturdifferenz > X °C innerhalb von 1 Stunde)  
  **Zweck:** Frühwarnsysteme für Frostgefahr  
- Live-Berechnung der gefühlten Temperatur pro Region (Temperatur- und Luftfeuchtigkeitswerte)  
  **Zweck:** Erkennen von Hitzewellen in Echtzeit

## Pattern: Classification of time interval

> Classify a certain time interval based on characteristics derived from the observed values within the interval.

**Examples:**
* Hitzeperioden bestimmen
  -> P(f(x_t,...,x_(t-n))

**Use Cases:**

- Real time recommendationn for outdoor activities  
- Heatwave Alerts  
- Real-time Severe Weather Alerts  
- Cold hail detection  
- Analyse von UV-Belastung (Schutz für unsere schöne Haut)  
- Erkennung von und Warnung vor Extremwetterlagen  
- Datenaufbereitung für Paragleiter (Wind, Luftdruck)  
- Hitze- oder Kälteperioden erkennen (ab x Tagen)  
- Erkennung von Waldbrandrisiken (Kombination von Temperatur, Wind, Luftfeuchtigkeit zur Risikoabschätzung)  
- Analyse von Temperatur und Feuchtigkeit zur Vorhersage von Mückenplagen oder Pollenflug  
- Frühwarnsysteme für Unwetter (z. B. Gewitter in 2 Tagen)  
- Nebelwarnung (vor allem für Abendverkehr)  
- Blitzeis-Warnung (für Auto- und Flugverkehr)  

## Pattern: Summary Statistics derived by comparing values within multiple intervals

> Calculate basic summary statistics (min, max, count, average) of values derived by functions that take at least two sets of values as parameters.

**Examples**

* Durchschnittliche Regendauer im Jahr

**Use Cases:**

- Höchste Temperaturen in der Zeitaufteilung 0-4h 4-8h 8-12h 12-16h 16-20h 20-0h, mit Wetter Typ für jede Wetter Station  
  **Zweck:** Wie haben sich die Klimas, im Laufe der Zeit auf Bezug der Höchsttemperaturen geändert. (interessant für Klimastatistiken)  
- Datenaufbereitung zur Neuschneeentwicklung (Niederschlag, Temperatur)  

## Pattern: Summary Statistics based on ordered values over Interval

> Calculate summary statistics that rely on ordered values (e.g. median, percentiles) over a given time interval.

**Examples**

* Median und Perzentile pro Jahr

## Pattern: Simple Forecasting 

> Calculate forecasts for a series of values based on historical values using simple methods such as moving averages, exponential smoothing, ...

**Examples**

* Was ist die voraussichtliche Durchschnittstemperatur in den nächsten 10 Jahren basierend auf der Steigung der letzten 10?

**Use Cases:**

- Durchschnittstemperatur-Berechnung: Gleitenden Durchschnitt der Temperatur.  
- Vorhersagen treffen basierend auf den letzten 1 oder mehr (2,3,4?) Wetterdaten (ML oder gleitender Mittelwert)  
- Wettervorhersage (anhand der letzten x Tage für die nächsten y Tage - update nach z Tagen)  
- Energy demand based on heat

### FTP Data Source

host: ftp.ncdc.noaa.gov
user: anonymous
password: password