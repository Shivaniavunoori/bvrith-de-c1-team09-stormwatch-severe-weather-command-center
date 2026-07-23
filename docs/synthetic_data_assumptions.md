# Synthetic Data Assumptions

**Project:** StormWatch -- Weather Event Analytics Platform\
**Week:** 2\
**Purpose:** Document the assumptions used for generating synthetic
weather event and storm monitoring data.

------------------------------------------------------------------------

# 1. Synthetic Data Boundary

This project uses **synthetically generated weather event data** for
educational purposes only.

The dataset does **not** represent any real meteorological agency,
government organization, weather station, citizen, location, or
historical weather event.

All Event IDs, Episode IDs, State Names, County/Zone Names, Alert IDs,
Locations, Fatality Records, and Streaming Alerts are fictional and
generated solely for learning Data Engineering concepts.

------------------------------------------------------------------------

# 2. Domain Assumptions

  -----------------------------------------------------------------------
  Area                    Assumption
  ----------------------- -----------------------------------------------
  Geography / Scope       Weather events occur across fictional states
                          and county/zones created for the StormWatch
                          platform.

  Time Period             Historical weather events are generated during
                          the **2025 weather season**, while streaming
                          alerts simulate near real-time monitoring.

  Source Systems          Storm Event Management, Location Tracking,
                          Fatality Reporting, Geography Reference, Event
                          Type Reference, and Streaming Alert Generator.

  Event Types             Thunderstorm Wind, Tornado, Hail, Flood, Flash
                          Flood, Lightning, Heavy Rain, Winter Storm,
                          High Wind, Dense Fog and other severe weather
                          events.

  Reference Data          State & County reference data, Event Type
                          reference data, Hazard Groups, Severity Levels,
                          and Alert metadata.
  -----------------------------------------------------------------------

------------------------------------------------------------------------

# 3. Data Volume Assumptions

  ----------------------------------------------------------------------------------------------
  File                                                        Approximate Rows Reason
  ------------------------------------ --------------------------------------- -----------------
  storm_event_details_2025.csv.gz                                     \~50,000 Primary weather
                                                                               event dataset
                                                                               used for
                                                                               analytics

  storm_event_locations_2025.csv.gz                                   \~72,080 Stores one or
                                                                               more locations
                                                                               for each weather
                                                                               event

  storm_event_fatalities_2025.csv.gz                                     \~850 Fatality records
                                                                               linked to storm
                                                                               events

  state_county_reference.csv                                             \~240 Geography
                                                                               reference dataset

  event_type_reference.csv                                                \~24 Weather event
                                                                               lookup dataset

  storm_alert_drop_01.json                                               \~100 Initial streaming
                                                                               alert events

  storm_alert_drop_02.json                                               \~100 Incremental
                                                                               streaming alert
                                                                               events
  ----------------------------------------------------------------------------------------------

------------------------------------------------------------------------

# 4. Controlled Data Quality Issues

  -----------------------------------------------------------------------
  Issue Type                     Approx. Share Why Include It
  ------------------- ------------------------ --------------------------
  Duplicate Event IDs               0.2%--0.5% Tests uniqueness
                                               validation

  Missing Mandatory                     1%--3% Tests completeness rules
  Values                                       

  Invalid Reference                   0.5%--1% Tests referential
  Keys                                         integrity

  Invalid Geographic                0.2%--0.5% Tests lookup validation
  Codes                                        

  Invalid Magnitude                 0.1%--0.5% Tests range validation
  Values                                       

  Timestamp                         0.1%--0.3% Tests chronology
  Inconsistencies                              validation

  Invalid Event Type                0.2%--0.5% Tests business rule
  Mapping                                      validation

  Malformed Streaming     Small controlled set Tests streaming schema
  Alerts                                       validation and quarantine
                                               logic
  -----------------------------------------------------------------------

------------------------------------------------------------------------

# 5. Manual Verification

-   Verify source files are generated successfully.
-   Verify row counts are within expected ranges.
-   Verify primary and foreign key consistency.
-   Verify timestamps and geographic mappings.
-   Verify controlled data quality issues remain limited.
-   Verify streaming events follow the expected schema.

------------------------------------------------------------------------

# 6. Notes

-   All datasets are synthetic.
-   Intended for educational Data Engineering use.
-   Supports Bronze, Silver, Gold, Quarantine and Streaming layers.


