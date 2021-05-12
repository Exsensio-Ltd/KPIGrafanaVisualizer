### OEE Grafana Plugin
The plugin built with React.js for Grafana Panel and provides representation of the  results of OEE (Overall Equipment Effectiveness) for specific device in bar chart.

The plugin has a few options that influence to the data that represented in the bar chart: Product, Station, Production period.

OEE values are divided by the production time (the time that equipment is expected to produce). A bar show a value of OEE for the selected production time that can be from 1 to 8 hours. Every bar is divided to the colored areas (red, yellow and green) that visualise the status of the OEE result. Each color is indicate the result: red is a bad (from 0 to 50), yellow is a satisfactory (from 50 to 75) and green is a good result (from 75).

#### Instalation and usage
1. Install dependencies
`yarn install`
2. Build plugin in production mode
`yarn build`
3. Place the build to the Grafana plugin folder
4. On the Grafana dashboard add a panel
5. Under the panel visualisation select the `OEE`
6. In the **Display** section set the `Base URL`. The URL of the Fiware orion brocker. By default the plugin will use `http://localhost:1026`
