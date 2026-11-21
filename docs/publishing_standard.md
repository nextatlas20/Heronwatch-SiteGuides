# Publishing standard — 2027 site guide

The 2027 edition covers the whole of 2027 and closes on **2027-12-31**. A site is
allowed into the edition only if the society can still stand behind the access
arrangements and the survey for the whole of that window.

## Four conditions

A site may be published when **all four** of the following hold:

1. `access.md` is present in the site folder.
2. `photos/` in the site folder holds **at least 3** files.
3. The volunteer portal's `last_survey` for the site is **2025-01-01 or later**.
4. The volunteer portal's `permit_expires` for the site is **2027-12-31 or later**.

## Blocker codes

A site that fails any condition is held, and every condition it fails is reported
with one of these codes:

| code | meaning |
| --- | --- |
| `access_missing` | there is no `access.md` in the site folder |
| `photos_insufficient` | `photos/` holds fewer than 3 files |
| `survey_stale` | the portal's `last_survey` is earlier than 2025-01-01 |
| `permit_expired` | the portal's `permit_expires` is earlier than 2027-12-31 |
| `no_portal_record` | the portal export has no row for the site at all |

`no_portal_record` stands alone: without a portal row neither date condition can be
judged, so no date code is reported alongside it.

Codes are reported in alphabetical order, joined with a comma and a single space.

## Where the facts come from

The site folders are the editorial record: they decide which sites exist, whether
`access.md` has been written and how many photographs are cleared.

The volunteer portal export is the administrative record and is the only authority for
`last_survey` and `permit_expires`. The `field_surveyed` and `field_permit_expires`
values typed into `overview.md` are the volunteer's field notes; they are frequently
stale and are never used for a publishing decision.
