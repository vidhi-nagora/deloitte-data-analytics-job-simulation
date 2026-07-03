# Manufacturing Telemetry Analysis (Tableau)

## Objective

Analyze telemetry data collected from four Daikibo manufacturing factories to identify:

- The factory with the highest machine downtime.
- The machine type responsible for the highest downtime.

---

## Tools Used

- Tableau
- JSON Dataset

---

## Approach

- Imported the telemetry JSON dataset into Tableau.
- Created a calculated field (`Unhealthy`) to estimate downtime.
- Built an interactive dashboard consisting of:
  - Downtime per Factory
  - Downtime per Device Type
- Applied dashboard filters to analyze machine downtime for each factory.

---

## Key Insight

The dashboard identifies the factory experiencing the highest downtime and highlights the machine type contributing most to the downtime.
