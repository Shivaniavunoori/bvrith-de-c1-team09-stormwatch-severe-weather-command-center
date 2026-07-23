# Data Dictionary

## event_type_reference.csv

|Field|Type|Nullable|Example|Description|
|---|---|---|---|---|
|event_type|STRING|N|Thunderstorm Wind|Controlled event-type key.|
|hazard_group|STRING|N|Convective|Broader hazard group.|
|magnitude_applicable_flag|STRING Y/N|N|Y|Whether magnitude is expected.|
|allowed_magnitude_type|STRING|Y|KT|Allowed magnitude unit/type.|
|high_impact_threshold|DECIMAL|N|58.0|Reference threshold used only as a modelling aid; students still derive approved severity.|
|default_severity_weight|DECIMAL|N|1.4|Synthetic modelling weight, not a final KPI.|
|synthetic_record_flag|STRING Y/N|N|Y|Y for every supplied record.|

## state_county_reference.csv

|Field|Type|Nullable|Example|Description|
|---|---|---|---|---|
|state_code|STRING|N|SW01|Fictional operating-region code.|
|state_name|STRING|N|North Coast|Fictional operating-region label.|
|region_group|STRING|N|Coastal|Broader geographic grouping.|
|county_zone_code|STRING|N|Z001|Fictional county/zone code.|
|county_zone_name|STRING|N|North Coast Zone 01|Fictional county/zone label.|
|centroid_latitude|DECIMAL|N|44.49471|Synthetic centroid latitude.|
|centroid_longitude|DECIMAL|N|-121.92881|Synthetic centroid longitude.|
|active_flag|STRING Y/N|N|Y|Reference active flag.|
|synthetic_record_flag|STRING Y/N|N|Y|Y for every supplied record.|

## storm_alert_drop_01/02.json

|Field|Type|Nullable|Example|Description|
|---|---|---|---|---|
|event_id|STRING|N|ALTEVT00001|Unique alert-transition event identifier.|
|schema_version|STRING|N|1.0|Expected 1.0.|
|event_ts|STRING ISO-8601 UTC|N|2026-01-15T12:00:00Z|Event-time timestamp.|
|event_type|STRING|N|storm_alert_transition|storm_alert_transition.|
|alert_id|STRING|N|ALT00001|Alert lifecycle identifier.|
|source_event_id|STRING|Y|EVT0020365|Optional link to batch event.|
|episode_id|STRING|Y|EPI012145|Optional episode link.|
|state_code|STRING|N|SW02|Fictional region code.|
|county_zone_code|STRING|N|Z028|Fictional zone code.|
|latitude|DECIMAL|N|46.51008|Synthetic latitude.|
|longitude|DECIMAL|N|-123.04199|Synthetic longitude.|
|hazard_type|STRING|N|Tornado|Alert hazard category.|
|severity|STRING|N|EXTREME|MINOR/MODERATE/SEVERE/EXTREME.|
|urgency|STRING|N|FUTURE|FUTURE/EXPECTED/IMMEDIATE.|
|certainty|STRING|N|POSSIBLE|POSSIBLE/LIKELY/OBSERVED.|
|previous_status|STRING|Y|nan|Prior lifecycle status.|
|new_status|STRING|N|ISSUED|ISSUED/UPDATED/ESCALATED/EXPIRED.|
|headline_code|STRING|N|HDR_EXCESSIVE_HEAT|Synthetic headline category.|
|alert_sequence_no|INTEGER|N|1|Ordered sequence within alert lifecycle.|
|producer_run_id|STRING|N|RUN_STREAM_01|Producer run lineage.|
|synthetic_record_flag|STRING Y/N|N|Y|Y for every valid JSON object.|

## storm_event_details_2025.csv.gz

|Field|Type|Nullable|Example|Description|
|---|---|---|---|---|
|source_record_id|STRING|N|SRC_EVT_0000001|Unique physical source-row identifier used for reconciliation.|
|event_id|STRING|N|EVT0000001|Storm event business identifier; expected unique at trusted event grain.|
|episode_id|STRING|N|EPI000001|Groups related storm events.|
|state_code|STRING|N|SW11|Fictional operating-region code.|
|state_name|STRING|N|Pine Highlands|Fictional operating-region label.|
|county_zone_code|STRING|N|Z213|Fictional county/zone code.|
|county_zone_name|STRING|N|Pine Highlands Zone 13|Fictional county/zone label.|
|event_type|STRING|N|Heavy Snow|Controlled severe-weather event type.|
|hazard_group|STRING|N|Winter|Broader hazard family.|
|begin_datetime|STRING ISO-8601 UTC|N|2025-05-14T10:34:25Z|Event start timestamp.|
|end_datetime|STRING ISO-8601 UTC|N|2025-05-22T02:50:25Z|Event end timestamp.|
|source_type|STRING|N|Trained Spotter|Synthetic reporting-source category.|
|magnitude|DECIMAL text-compatible|Y|0.77|Magnitude value when applicable to the event type.|
|magnitude_type|STRING|Y|IN|Unit/type for magnitude.|
|injuries_direct|INTEGER|N|0|Synthetic direct injury count.|
|injuries_indirect|INTEGER|N|0|Synthetic indirect injury count.|
|fatalities_direct|INTEGER|N|0|Synthetic direct fatality count at event grain.|
|fatalities_indirect|INTEGER|N|0|Synthetic indirect fatality count at event grain.|
|damage_property_text|STRING|Y|0|Reported property damage text using zero/K/M/B conventions.|
|damage_crops_text|STRING|Y|0|Reported crop damage text using zero/K/M/B conventions.|
|event_narrative|STRING|N|Synthetic heavy snow training event in Pine Highlands Zone 13; no real incident or person is represented.|Synthetic narrative with no person or real incident.|
|synthetic_record_flag|STRING Y/N|N|Y|Y for every supplied record.|

## storm_event_fatalities_2025.csv.gz

|Field|Type|Nullable|Example|Description|
|---|---|---|---|---|
|source_record_id|STRING|N|SRC_FAT_000001|Unique physical source-row identifier.|
|fatality_id|STRING|N|FAT000001|Fatality-record identifier; not a person identifier.|
|event_id|STRING|N|EVT0000172|Parent event identifier.|
|fatality_type|STRING|N|Indirect|Direct or Indirect.|
|fatality_date|STRING ISO-8601 UTC|N|2025-02-24T22:14:07Z|Synthetic event-linked fatality timestamp.|
|age_band|STRING|N|35-49|Privacy-safe age bucket.|
|sex_category|STRING|N|Male|Broad category including unknown/not reported.|
|fatality_location_category|STRING|N|Unknown/Other|Broad location category.|
|privacy_bucket_flag|STRING Y/N|N|Y|Y confirms bucketed treatment.|
|synthetic_record_flag|STRING Y/N|N|Y|Y for every supplied record.|

## storm_event_locations_2025.csv.gz

|Field|Type|Nullable|Example|Description|
|---|---|---|---|---|
|source_record_id|STRING|N|SRC_LOC_00000001|Unique physical source-row identifier.|
|location_id|STRING|N|LOC00000001|Location record identifier.|
|event_id|STRING|N|EVT0000001|Parent event identifier.|
|location_index|INTEGER|N|1|Sequence within the event.|
|state_code|STRING|N|SW11|Fictional operating-region code.|
|county_zone_code|STRING|N|Z213|Fictional county/zone code.|
|latitude|DECIMAL|N|32.65051|Synthetic coordinate for engineering validation only.|
|longitude|DECIMAL|N|-81.97436|Synthetic coordinate for engineering validation only.|
|location_type|STRING|N|Point|Point/path/zone category.|
|path_length_km|DECIMAL|N|4.06|Synthetic path length.|
|path_width_km|DECIMAL|N|0.22|Synthetic path width.|
|location_name|STRING|N|Pine Highlands Zone 13 Sector 1|Fictional zone/sector label.|
|synthetic_record_flag|STRING Y/N|N|Y|Y for every supplied record.|



