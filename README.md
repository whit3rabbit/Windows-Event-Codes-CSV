# Windows Event Codes CSV

This project scrapes Windows Event Logs from the Ultimate Windows Security website and processes them into a CSV file.

## Open in Google Colab

You can open the notebook in Google Colab by clicking the badge below:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/whit3rabbit/windows_event_codes_csv/blob/main/Windows_Event_Logs.ipynb)

## Output Files

### detailed_events.csv
This file contains detailed information about each Windows Event Log entry, including:
- **Source**: The source of the event.
- **Event_ID**: The unique identifier for the event.
- **Event Summary**: A brief summary of the event.
- **URL**: The URL where more information about the event can be found.
- **Operating Systems**: The operating systems that the event applies to.
- **Category and Subcategory**: The category and subcategory of the event.
- **Type**: The type of event.
- **Description**: A detailed description of the event.
- **Event Example**: An example of the event.

### updated_detailed_events.csv
This file is an updated version of `detailed_events.csv` with additional information merged from Microsoft's recommendations. It includes:
- **Current_Event_ID**: The current event ID.
- **Legacy_Event_ID**: The legacy event ID, normalized and expanded.
- **Potential_Criticality**: The potential criticality of the event.
- **Event_Summary**: A summary of the event, updated if necessary.
- **Operating Systems**: Cleaned and standardized operating system information.
- **Description**: Cleaned descriptions with specific text patterns removed.
