# Local API simulation

These files are teaching fixtures, not a running API. No live service, authentication or network is needed.

Example request: GET /actions?completed=false.
Conceptual response: a status code, headers and a body. Status describes the request outcome; the body contains data that still needs validation.

- [success.json](success.json): simulated status 200 and two open actions. Expected report: 2 open actions, one each for Alex and Sam.
- [empty.json](empty.json): simulated status 200 and no actions. Expected: “No open actions.”
- [unavailable.json](unavailable.json): simulated status 503. Expected: an explicit unavailable-source message; do not claim a complete current report or silently use stale data.

Do not send requests to an invented hostname. For a live extension, choose a documented public read-only API, verify its current official docs, limits and terms, and preserve the offline fixture path.

The same schema validation used for local data should also be applied to a live response. A successful HTTP status does not prove the records are valid.
