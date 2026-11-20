# AAPMIS 2.0 app summary

Reviewed in the Power Apps maker portal on 2026-11-20 in the `dev-jts745` environment.

Source: [AAPMIS Core solution](https://make.powerapps.com/environments/43f231dd-2458-e4de-8f46-d3c629f1f9f2/solutions/63ce6086-9976-47a3-bc02-1a3d701d82e0/objects/apps). See [AAPMIS data model](AAPMIS-data-model.md) for table columns, data types, and relationships.

## Purpose and platform

**Athlete Assistance Program Management Information System (AAPMIS) 2.0** is an enabled model-driven Power App (`pch_AAPMIS20`) in the **AAPMIS Core** solution. Its settings describe it as a way to organize and track key provincial information for operational oversight. It uses Dataverse tables, views, forms, and a site map.

The solution is unmanaged, version `1.0.0.1`, with publisher `pch`. The app is owned by Elliot Chen. Offline use is disabled in the app settings.

## User navigation

| Area | Pages visible in the app |
| --- | --- |
| NSO & Sports Management | National Sport Organizations; NSO Contacts |
| Athlete Management | Athletes |

The app designer also lists views and forms for **Sport (Obsolete)** under “All other pages”; they are not in the configured navigation. The user interface provides standard model-driven search, record creation, filtering, and list commands.

## Configured forms and views

| Page | What was visible in the designer preview |
| --- | --- |
| National Sport Organizations | The active list has English and French names, phone, email, address, province, city, and postal code columns. The new-record form has required English and French names, contact and address fields, a Province lookup, notes, and an Audit tab. |
| NSO Contacts | The active list has Name and Created On columns. The new-record form showed only Owner, despite additional contact columns existing in the table schema. |
| Athletes | The active list has Name and Created On columns. The new-record form showed Name and Owner, despite a substantially broader athlete table schema. |

Each of those active lists showed **zero rows in the designer preview** during the review. No records were created or changed, so existing-record behavior and save validation were not tested.

## Data and solution components

The solution contains **12 tables**, including eight custom AAPMIS tables and four Microsoft platform tables. The eight custom tables are Athlete, Athlete Address, IPC Classification, National Sport Organization, NSO Contact, Province, Sport (Obsolete), and Sport Discipline. It also includes seven choices, seven security roles, and one site map. No cloud flows are included in the solution.

The app designer's Automation panel listed three business process flows: **Expired Process**, **New Process**, and **Translation Process**. Their behavior was not tested. The designer showed a prompt to enable Copilot, so Copilot was not observed as an active app feature.

## Review observations

1. **Form coverage is uneven.** The NSO form exposes several business fields; the Athlete and NSO Contact forms expose only minimal fields in the designer preview. Their underlying Dataverse tables contain more columns. Confirm the intended forms and views before relying on the app for full data entry.
2. **An environment variable needs a value.** The solution overview reports one environment variable requiring an update: `Lookup Localization Config`, described as JSON configuration for the Lookup Localization plugin.
3. **Solution Checker has not been run.** The overview reported no Solution Checker result at the time of review.
4. **Business links are limited.** The inspected data model has five direct business relationships. In particular, no direct Athlete-to-NSO relationship appeared in the custom table relationship grids. See the linked data model for the full map.

This is a review of maker-portal configuration and preview, not a functional acceptance test or a review of live user data.
