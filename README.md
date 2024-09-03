# NOAA Space Weather Dashboard

## Overview
This repository contains the necessary configurations and resources to set up a Grafana dashboard displaying 24-Hour Observed Maximums for space weather conditions based on NOAA scales. The dashboard provides a visual representation of the current space weather, including geomagnetic storms, solar radiation storms, and radio blackouts, updated dynamically from NOAA data.

![NOAA Space Weather Dashboard](screenshot/Screenshot 2024-09-02 at 20.22.47.png)

## Setup Instructions

### Setting Up Telegraf
1. **Install Telegraf**: If not already installed, download and install Telegraf from [InfluxData](https://portal.influxdata.com/downloads/).
2. **Configure Telegraf**: Copy the configuration file from `telegraf.d/` into your Telegraf directory.
3. **Start Telegraf**: Run Telegraf using the command `telegraf --config telegraf.d/<filename>`

### Importing Dashboard into Grafana
1. **Open Grafana**: Log in to your Grafana instance.
2. **Import Dashboard**: Navigate to the dashboard import section (`+` > `Import`).
3. **Upload JSON File**: Use the `noaa_space.json` file from this repository to import the dashboard.
