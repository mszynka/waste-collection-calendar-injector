# waste-collection-calendar-injector

![Waste disposal automation](Waste%20disposal%20automation.png)

This Node-RED flow automates the process of adding waste collection schedules to a Home Assistant calendar. It fetches data from the API at [https://zys-harmonogram.smok.net.pl/](https://zys-harmonogram.smok.net.pl/), extracts the waste collection timetable, and creates events in your selected Home Assistant calendar.

It should work with [https://www.puk-zys.pl/index.php/harmonogram-wywozow/](https://www.puk-zys.pl/index.php/harmonogram-wywozow/) for both Kleszczewo and Kostrzyn region.

## Features

- Scrapes the waste collection schedule for a specified region and year.
- Handles sorting by waste types, including mixed, recyclable, and special categories like Christmas trees.
- Adds waste collection events to your Home Assistant calendar, ensuring you're always up-to-date.

## Requirements

- A working Home Assistant instance with an available calendar integration.
- Node-RED integrated with Home Assistant
- Environment variables for `region` and `year` to specify the location and time frame.

## Usage

1. Import the nodered-flow.json flow into your Node-RED instance.
2. Update the `region` and `year` variables in the flow to match your location and desired schedule year.
3. Deploy the flow in Node-RED.
4. Watch as waste collection events are automatically added to your chosen Home Assistant calendar.
