---
swagger: "2.0"
info:
  title: Weatherbit Get History Energy Lat & Lon
  description: Returns aggregate energy specific historical weather fields, over a
    specified time period.
  version: 2.0.0
host: api.weatherbit.io
basePath: /v2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /history/energy?lat={lat}&lon={lon}:
    get:
      summary: Get History Energy Lat & Lon
      description: Returns aggregate energy specific historical weather fields, over
        a specified time period
      operationId: returns-aggregate-energy-specific-historical-weather-fields-over-a-specified-time-period
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: end_date
        description: End Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: key
        description: Your registered API key
      - in: path
        name: lat
        description: Latitude component of location
      - in: path
        name: lon
        description: Longitude component of location
      - in: query
        name: start_date
        description: Start Date (YYYY-MM-DD or YYYY-MM-DD:HH)
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - weather
      - history
      - energy
      - lat
      - lat
      - '&lon'
      - lon
definitions:
  CurrentObs:
    properties:
      app_temp:
        description: This is a default description.
        type: get
      city_name:
        description: This is a default description.
        type: get
      clouds:
        description: This is a default description.
        type: get
      country_code:
        description: This is a default description.
        type: get
      datetime:
        description: This is a default description.
        type: get
      dewpt:
        description: This is a default description.
        type: get
      dhi:
        description: This is a default description.
        type: get
      elev_angle:
        description: This is a default description.
        type: get
      hour_angle:
        description: This is a default description.
        type: get
      lat:
        description: This is a default description.
        type: get
  CurrentObsGroup:
    properties:
      count:
        description: This is a default description.
        type: get
      data:
        description: This is a default description.
        type: get
  EnergyObs:
    properties:
      cdd:
        description: This is a default description.
        type: get
      city_name:
        description: This is a default description.
        type: get
      clouds:
        description: This is a default description.
        type: get
      country_code:
        description: This is a default description.
        type: get
      dewpt:
        description: This is a default description.
        type: get
      dhi:
        description: This is a default description.
        type: get
      hdd:
        description: This is a default description.
        type: get
      lat:
        description: This is a default description.
        type: get
      lon:
        description: This is a default description.
        type: get
      precip:
        description: This is a default description.
        type: get
  EnergyObsGroup:
    properties:
      count:
        description: This is a default description.
        type: get
      data:
        description: This is a default description.
        type: get
      end_date:
        description: This is a default description.
        type: get
      start_date:
        description: This is a default description.
        type: get
  Error:
    properties:
      code:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
  Forecast:
    properties:
      app_max_temp:
        description: This is a default description.
        type: get
      app_min_temp:
        description: This is a default description.
        type: get
      clouds:
        description: This is a default description.
        type: get
      datetime:
        description: This is a default description.
        type: get
      dewpt:
        description: This is a default description.
        type: get
      max_dhi:
        description: This is a default description.
        type: get
      max_temp:
        description: This is a default description.
        type: get
      min_temp:
        description: This is a default description.
        type: get
      pod:
        description: This is a default description.
        type: get
      pop:
        description: This is a default description.
        type: get
  ForecastDay:
    properties:
      city_name:
        description: This is a default description.
        type: get
      country_code:
        description: This is a default description.
        type: get
      data:
        description: This is a default description.
        type: get
      lat:
        description: This is a default description.
        type: get
      lon:
        description: This is a default description.
        type: get
      state_code:
        description: This is a default description.
        type: get
      timezone:
        description: This is a default description.
        type: get
  ForecastHour:
    properties:
      app_temp:
        description: This is a default description.
        type: get
      clouds:
        description: This is a default description.
        type: get
      datetime:
        description: This is a default description.
        type: get
      dewpt:
        description: This is a default description.
        type: get
      dhi:
        description: This is a default description.
        type: get
      pod:
        description: This is a default description.
        type: get
      pop:
        description: This is a default description.
        type: get
      precip:
        description: This is a default description.
        type: get
      precip6h:
        description: This is a default description.
        type: get
      pres:
        description: This is a default description.
        type: get
  ForecastHourly:
    properties:
      city_name:
        description: This is a default description.
        type: get
      country_code:
        description: This is a default description.
        type: get
      data:
        description: This is a default description.
        type: get
      lat:
        description: This is a default description.
        type: get
      lon:
        description: This is a default description.
        type: get
      state_code:
        description: This is a default description.
        type: get
      timezone:
        description: This is a default description.
        type: get
  GeoIPObj:
    properties:
      area_code:
        description: This is a default description.
        type: get
      charset:
        description: This is a default description.
        type: get
      city:
        description: This is a default description.
        type: get
      continent_code:
        description: This is a default description.
        type: get
      country_code:
        description: This is a default description.
        type: get
      country_code3:
        description: This is a default description.
        type: get
      dma_code:
        description: This is a default description.
        type: get
      ip:
        description: This is a default description.
        type: get
      latitude:
        description: This is a default description.
        type: get
      longitude:
        description: This is a default description.
        type: get
  History:
    properties:
      city_name:
        description: This is a default description.
        type: get
      country_code:
        description: This is a default description.
        type: get
      data:
        description: This is a default description.
        type: get
      lat:
        description: This is a default description.
        type: get
      lon:
        description: This is a default description.
        type: get
      state_code:
        description: This is a default description.
        type: get
      timezone:
        description: This is a default description.
        type: get
  HistoryDay:
    properties:
      city_name:
        description: This is a default description.
        type: get
      country_code:
        description: This is a default description.
        type: get
      data:
        description: This is a default description.
        type: get
      lat:
        description: This is a default description.
        type: get
      lon:
        description: This is a default description.
        type: get
      state_code:
        description: This is a default description.
        type: get
      timezone:
        description: This is a default description.
        type: get
  HistoryDayObj:
    properties:
      datetime:
        description: This is a default description.
        type: get
      dewpt:
        description: This is a default description.
        type: get
      dhi:
        description: This is a default description.
        type: get
      max_temp:
        description: This is a default description.
        type: get
      max_temp_ts:
        description: This is a default description.
        type: get
      max_uv:
        description: This is a default description.
        type: get
      max_wind_dir:
        description: This is a default description.
        type: get
      max_wind_spd:
        description: This is a default description.
        type: get
      max_wind_spd_ts:
        description: This is a default description.
        type: get
      min_temp:
        description: This is a default description.
        type: get
  HistoryObj:
    properties:
      datetime:
        description: This is a default description.
        type: get
      dewpt:
        description: This is a default description.
        type: get
      dhi:
        description: This is a default description.
        type: get
      elev_angle:
        description: This is a default description.
        type: get
      h_angle:
        description: This is a default description.
        type: get
      pod:
        description: This is a default description.
        type: get
      precip:
        description: This is a default description.
        type: get
      precip6h:
        description: This is a default description.
        type: get
      pres:
        description: This is a default description.
        type: get
      qc:
        description: This is a default description.
        type: get
x-collection-name: Weatherbit
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---