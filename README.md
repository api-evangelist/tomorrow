# Tomorrow.io (tomorrow)
Tomorrow.io is a weather and climate intelligence platform exposing a unified v4 HTTP API. The API combines real-time observations, hyperlocal forecast timelines (minutely / hourly / daily), 20+ years of historical data, climate normals, weather-on-routes, configurable insights and event detection, per-location alerts with webhook delivery, and raster map tiles. 60+ data layers cover core weather, air quality, pollen, fire, flood, soil, solar, aviation, maritime, and lightning.

**URL:** [Visit APIs.json URL](https://docs.tomorrow.io)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Weather, Climate, Forecast, Historical Weather, Air Quality, Pollen, Fire, Flood, Routes, Map Tiles, Aviation, Maritime, Public APIs

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-30

## APIs

### Tomorrow.io Weather API
Unified Tomorrow.io v4 HTTP API. Exposes Realtime weather, multi-step Timelines forecasts (minutely / hourly / daily), Historical data, Weather-on-Routes, raster Map Tiles, plus management surfaces for Locations, Insights, Alerts, and Events with configurable thresholds and webhook delivery.

**Human URL:** [https://docs.tomorrow.io/reference/welcome](https://docs.tomorrow.io/reference/welcome)

**Base URL:** `https://api.tomorrow.io/v4`

#### Tags:

 - Weather, Forecast, Climate, Routes, Map Tiles

#### Properties

- [Documentation](https://docs.tomorrow.io/reference/welcome)
- [OpenAPI](openapi/tomorrow-openapi.yml)
- [Postman](https://github.com/Tomorrow-IO-API/tomorrow-postman)
- [SignUp](https://app.tomorrow.io/signup)
- [Authentication](https://app.tomorrow.io/development/keys)
- [CodeExamples — JavaScript Samples](https://github.com/Tomorrow-IO-API/tomorrow-samples)
- [CodeExamples — Routes + Mapbox Sample](https://github.com/Tomorrow-IO-API/tomorrow-route-mapbox)
- [CodeExamples — Timelines Widget Sample](https://github.com/Tomorrow-IO-API/tomorrow-timelines-widget)
- [CodeExamples — Insights Dashboard Sample](https://github.com/Tomorrow-IO-API/tomorrow-events-charts)
- [CodeExamples — API Proxy (Google Cloud Function)](https://github.com/Tomorrow-IO-API/tomorrow-api-proxy)
- [CodeExamples — Netlify Function Sample](https://github.com/Tomorrow-IO-API/tomorrow-netlify)
- [CodeExamples — Climate Normals Visualization](https://github.com/Tomorrow-IO-API/climate-normals)
- [WeatherIcons](https://github.com/Tomorrow-IO-API/tomorrow-weather-codes)
- [MapAssets](https://github.com/Tomorrow-IO-API/tomorrow-map-spectrums)
- [NaftikoCapability](capabilities/tomorrow-alerts.yaml)
- [NaftikoCapability](capabilities/tomorrow-climate.yaml)
- [NaftikoCapability](capabilities/tomorrow-events.yaml)
- [NaftikoCapability](capabilities/tomorrow-forecast.yaml)
- [NaftikoCapability](capabilities/tomorrow-historical.yaml)
- [NaftikoCapability](capabilities/tomorrow-insights.yaml)
- [NaftikoCapability](capabilities/tomorrow-locations.yaml)
- [NaftikoCapability](capabilities/tomorrow-map-tiles.yaml)
- [NaftikoCapability](capabilities/tomorrow-realtime.yaml)
- [NaftikoCapability](capabilities/tomorrow-routes.yaml)
- [NaftikoCapability](capabilities/tomorrow-timelines.yaml)

## Common Properties

- [Website](https://www.tomorrow.io)
- [Documentation](https://docs.tomorrow.io)
- [Pricing](https://www.tomorrow.io/weather-api/)
- [SignUp](https://app.tomorrow.io/signup)
- [Authentication](https://app.tomorrow.io/development/keys)
- [GitHubOrganization](https://github.com/Tomorrow-IO-API)
- [GitHubOrganization — Tomorrow.io (corporate org)](https://github.com/tomorrowio)
- [Status](https://tomorrowio.statuspage.io)
- [Blog](https://www.tomorrow.io/blog/)
- [Community](https://github.com/Tomorrow-IO-API/tomorrow-community)
- [Support](https://www.tomorrow.io/support/)
- [ReleaseNotes](https://docs.tomorrow.io/changelog)
- [PublicAPIsListing](https://github.com/public-apis/public-apis)
- [Plans](plans/tomorrow-plans-pricing.yml)
- [RateLimits](rate-limits/tomorrow-rate-limits.yml)
- [FinOps](finops/tomorrow-finops.yml)
- [SpectralRuleset](rules/tomorrow-spectral-rules.yml)
- [Vocabulary](vocabulary/tomorrow-vocabulary.yml)
- [JSONLDContext](json-ld/tomorrow-weather-api-context.jsonld)

## Features

| Name | Description |
|------|-------------|
| 60+ Data Layers | Core weather plus air quality (EPA/MEP indices, particulates, pollutants), pollen (tree species, grass, weed), fire (FWI), solar (GHI/DIF/DIR), lightning, soil moisture/temperature, marine swell and wave, aviation ceiling/visibility, and road conditions. |
| Forecast Timelines | Single endpoint returns minutely (1m/5m/15m/30m), hourly (1h), daily (1d) and current timesteps for any combination of fields. Up to 14 days out on paid plans, 5 days on Free. |
| Historical Data | Up to 20 years of historical observations for the same field universe as the forecast, retrievable by point or polygon. |
| Climate Normals | 30-year climate normals (monthly averages) for any location, useful for anomaly detection and climate-trend reporting. |
| Weather on Routes | POST a polyline or list of waypoints and receive weather along the route at each segment with arrival-time interpolation. |
| Map Tiles | Raster tile endpoint `/map/tile/{z}/{x}/{y}/{field}/{timeFormat}` for Mapbox, Google Maps, Leaflet, OpenLayers, Cesium overlays. |
| Custom Insights and Events | Define threshold rules (e.g. windSpeed > 15 m/s AND precipitationProbability > 50%) against any field, then poll the Events endpoint for matches at a location or buffer. |
| Alerts with Webhooks | Persistent alert resources linked to one or more locations; activations fire to a webhook destination so downstream systems can react in real time. |
| Locations Management | CRUD on point, polygon, and polyline locations with tag-based grouping, so monitored assets can be addressed by ID instead of repeated geometry. |

## Use Cases

| Name | Description |
|------|-------------|
| Aviation Operations | Airlines use ceiling, visibility, wind shear, and storm cells along the route to make ground-stop, diversion, and de-icing decisions. |
| Logistics and Routing | Trucking, last-mile delivery, and rail use route-weather and lightning tracking to reroute shipments and reschedule outdoor crews. |
| Energy and Utilities | Wind, solar (GHI/DIF/DIR), and lightning data feed renewable forecasting, grid load planning, and outage prediction. |
| Agriculture | Soil moisture, soil temperature, evapotranspiration, and growing-degree days drive irrigation, planting, and spray-window decisions. |
| Insurance Underwriting and Claims | Historical hail, wind, and flood data inform underwriting; real-time hail and lightning detection accelerates claims triage. |
| Sports and Live Events | Stadium operators monitor lightning radius and precipitation probability to call delays and protect spectators. |
| Public Safety and Government | Fire weather (FWI), flood indices, and air-quality (EPA AQI) feed municipal alerting and emergency-management workflows. |
| Retail and CPG | Demand forecasting models use temperature anomalies and weekly weather patterns to plan inventory and promotions. |
| Maritime and Offshore | Wave height, swell direction, and wind data drive routing, port operations, and offshore platform safety windows. |

## Integrations

| Name | Description |
|------|-------------|
| Mapbox | Vector and raster basemaps overlaid with Tomorrow.io map tiles. |
| Google Maps | JavaScript Maps API overlay support. |
| Leaflet | Open-source web map tile overlay. |
| OpenLayers | GIS-grade web map library tile overlay. |
| Cesium | 3D globe / aviation tile overlay. |
| Postman | Official Tomorrow.io Postman collection. |
| Webhooks | Alert activations delivered to any HTTP endpoint. |

## Solutions

| Name | Description |
|------|-------------|
| Aviation Weather Intelligence | Route weather, turbulence, icing, ceiling and visibility for flight planning. |
| Resilience for Logistics | Lightning, hail, and severe-weather alerting for fleets and warehouses. |
| Renewable Energy Forecasting | Wind and solar generation forecasts with multi-day timelines and historical baselining. |
| Climate Risk for Insurance | Historical perils + climate-normal anomalies for underwriting and CAT modeling. |
| Agriculture Decision Support | Soil + growing-condition data for irrigation, planting, and spraying. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [tomorrow-openapi](openapi/tomorrow-openapi.yml)

### Postman

- [tomorrow-postman-collection](postman/tomorrow-postman-collection.json)

### JSON Schema (27 files)

- [alert-create-request-schema](json-schema/alert-create-request-schema.json)
- [alert-location-link-request-schema](json-schema/alert-location-link-request-schema.json)
- [alert-schema](json-schema/alert-schema.json)
- [climate-normals-request-schema](json-schema/climate-normals-request-schema.json)
- [climate-normals-response-schema](json-schema/climate-normals-response-schema.json)
- [event-schema](json-schema/event-schema.json)
- [events-request-schema](json-schema/events-request-schema.json)
- [events-response-schema](json-schema/events-response-schema.json)
- [forecast-response-schema](json-schema/forecast-response-schema.json)
- [geo-jsongeometry-schema](json-schema/geo-jsongeometry-schema.json)
- [historical-request-schema](json-schema/historical-request-schema.json)
- [insight-condition-schema](json-schema/insight-condition-schema.json)
- [insight-create-request-schema](json-schema/insight-create-request-schema.json)
- [insight-schema](json-schema/insight-schema.json)
- [location-create-request-schema](json-schema/location-create-request-schema.json)
- [location-schema](json-schema/location-schema.json)
- [location-tags-request-schema](json-schema/location-tags-request-schema.json)
- [location-update-request-schema](json-schema/location-update-request-schema.json)
- [realtime-weather-response-schema](json-schema/realtime-weather-response-schema.json)
- [route-request-schema](json-schema/route-request-schema.json)
- [route-response-schema](json-schema/route-response-schema.json)
- [route-waypoint-schema](json-schema/route-waypoint-schema.json)
- [timeline-interval-schema](json-schema/timeline-interval-schema.json)
- [timeline-schema](json-schema/timeline-schema.json)
- [timelines-request-schema](json-schema/timelines-request-schema.json)
- [timelines-response-schema](json-schema/timelines-response-schema.json)
- [weather-values-schema](json-schema/weather-values-schema.json)

### JSON Structure (27 files)

- [alert-create-request-structure](json-structure/alert-create-request-structure.json)
- [alert-location-link-request-structure](json-structure/alert-location-link-request-structure.json)
- [alert-structure](json-structure/alert-structure.json)
- [climate-normals-request-structure](json-structure/climate-normals-request-structure.json)
- [climate-normals-response-structure](json-structure/climate-normals-response-structure.json)
- [event-structure](json-structure/event-structure.json)
- [events-request-structure](json-structure/events-request-structure.json)
- [events-response-structure](json-structure/events-response-structure.json)
- [forecast-response-structure](json-structure/forecast-response-structure.json)
- [geo-jsongeometry-structure](json-structure/geo-jsongeometry-structure.json)
- [historical-request-structure](json-structure/historical-request-structure.json)
- [insight-condition-structure](json-structure/insight-condition-structure.json)
- [insight-create-request-structure](json-structure/insight-create-request-structure.json)
- [insight-structure](json-structure/insight-structure.json)
- [location-create-request-structure](json-structure/location-create-request-structure.json)
- [location-structure](json-structure/location-structure.json)
- [location-tags-request-structure](json-structure/location-tags-request-structure.json)
- [location-update-request-structure](json-structure/location-update-request-structure.json)
- [realtime-weather-response-structure](json-structure/realtime-weather-response-structure.json)
- [route-request-structure](json-structure/route-request-structure.json)
- [route-response-structure](json-structure/route-response-structure.json)
- [route-waypoint-structure](json-structure/route-waypoint-structure.json)
- [timeline-interval-structure](json-structure/timeline-interval-structure.json)
- [timeline-structure](json-structure/timeline-structure.json)
- [timelines-request-structure](json-structure/timelines-request-structure.json)
- [timelines-response-structure](json-structure/timelines-response-structure.json)
- [weather-values-structure](json-structure/weather-values-structure.json)

### JSON-LD

- [tomorrow-weather-api-context](json-ld/tomorrow-weather-api-context.jsonld)

### Examples (27 files)

- [alert-create-request-example](examples/alert-create-request-example.json)
- [alert-example](examples/alert-example.json)
- [alert-location-link-request-example](examples/alert-location-link-request-example.json)
- [climate-normals-request-example](examples/climate-normals-request-example.json)
- [climate-normals-response-example](examples/climate-normals-response-example.json)
- [event-example](examples/event-example.json)
- [events-request-example](examples/events-request-example.json)
- [events-response-example](examples/events-response-example.json)
- [forecast-response-example](examples/forecast-response-example.json)
- [geo-jsongeometry-example](examples/geo-jsongeometry-example.json)
- [historical-request-example](examples/historical-request-example.json)
- [insight-condition-example](examples/insight-condition-example.json)
- [insight-create-request-example](examples/insight-create-request-example.json)
- [insight-example](examples/insight-example.json)
- [location-create-request-example](examples/location-create-request-example.json)
- [location-example](examples/location-example.json)
- [location-tags-request-example](examples/location-tags-request-example.json)
- [location-update-request-example](examples/location-update-request-example.json)
- [realtime-weather-response-example](examples/realtime-weather-response-example.json)
- [route-request-example](examples/route-request-example.json)
- [route-response-example](examples/route-response-example.json)
- [route-waypoint-example](examples/route-waypoint-example.json)
- [timeline-example](examples/timeline-example.json)
- [timeline-interval-example](examples/timeline-interval-example.json)
- [timelines-request-example](examples/timelines-request-example.json)
- [timelines-response-example](examples/timelines-response-example.json)
- [weather-values-example](examples/weather-values-example.json)

## Capabilities

Self-contained Naftiko capabilities — one per OpenAPI tag — each declaring REST and MCP exposers over an inline `consumes` block.

### Tomorrow.io Weather API

| Capability | Tools |
|---|---|
| [Tomorrow.io Weather API — Alerts](capabilities/tomorrow-alerts.yaml) | 10 |
| [Tomorrow.io Weather API — Climate](capabilities/tomorrow-climate.yaml) | 1 |
| [Tomorrow.io Weather API — Events](capabilities/tomorrow-events.yaml) | 2 |
| [Tomorrow.io Weather API — Forecast](capabilities/tomorrow-forecast.yaml) | 1 |
| [Tomorrow.io Weather API — Historical](capabilities/tomorrow-historical.yaml) | 1 |
| [Tomorrow.io Weather API — Insights](capabilities/tomorrow-insights.yaml) | 5 |
| [Tomorrow.io Weather API — Locations](capabilities/tomorrow-locations.yaml) | 7 |
| [Tomorrow.io Weather API — Map Tiles](capabilities/tomorrow-map-tiles.yaml) | 1 |
| [Tomorrow.io Weather API — Realtime](capabilities/tomorrow-realtime.yaml) | 1 |
| [Tomorrow.io Weather API — Routes](capabilities/tomorrow-routes.yaml) | 1 |
| [Tomorrow.io Weather API — Timelines](capabilities/tomorrow-timelines.yaml) | 2 |

## Vocabulary

- [Tomorrow.io Vocabulary](vocabulary/tomorrow-vocabulary.yml) — Unified taxonomy mapping 11 resources, 12 actions, 11 workflows, and 7 personas across operational (OpenAPI) and capability (Naftiko) dimensions.

## Rules

- [tomorrow-spectral-rules](rules/tomorrow-spectral-rules.yml) — 42 Spectral rules enforcing Tomorrow.io API conventions.

## Plans

- [tomorrow-plans-pricing](plans/tomorrow-plans-pricing.yml)

## Rate Limits

- [tomorrow-rate-limits](rate-limits/tomorrow-rate-limits.yml)

## FinOps

- [tomorrow-finops](finops/tomorrow-finops.yml)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
