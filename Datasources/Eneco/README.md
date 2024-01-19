# Energy provider: Eneco

Eneco offers the option to export data from their website (Mijn Eneco). This data can be transformed and used to import into Home Assistant.

**Data provided**
- Electricity consumption - Tariff 1 - High resolution (day interval) - kWh
- Electricity consumption - Tariff 2 - High resolution (day interval) - kWh
- Electricity production - Tariff 1 - High resolution (day interval) - kWh
- Electricity production - Tariff 2 - High resolution (day interval) - kWh

**Tooling needed**
- Python 3
- Pandas python library ```pip install pandas```
- OpenPyXL python library ```pip install openpyxl```

**How-to**
- Export data from Eneco
- Download the ```EnecoDataPrepare.py``` file and put it in the same directory as the Eneco data
- Execute the python script with as parameter the name of the file that contains the exported data ```python EnecoPrepare.py "Verbruik_01-01-2020-31-12-2020.xlsx"```. The python script creates the needed files for the generic import script.
- Follow the steps in the overall how-to