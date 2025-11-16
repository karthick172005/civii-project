Civii API (initial)
- POST /api/v1/report/upload
  body: { reporter_id, category, lat, lon, timestamp, media_url or media file }
  returns: { report_id, status }

- GET /api/v1/reports?lat=&lon=&radius=&status=
  returns: list of nearby reports

- POST /api/v1/report/:id/status
  body: { status: 'pending'|'approved'|'rejected'|'solved', updater_id }

- GET /api/v1/admin/pending
  returns: list of reports pending approval
