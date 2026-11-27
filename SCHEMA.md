# data/projects.json schema

```
{
  "as_of": "YYYY-MM-DD",          // date the snapshot was taken (UTC)
  "source": "https://gtapcport.org/",
  "live_json": "https://gtapcport.org/_d/tracker/projects",
  "stages": [ ...6 stage names, index 0 = stage 1 ],
  "projects": [ Project, ... ]
}
```

## Project

| Field | Type | Description |
|---|---|---|
| `name` | string | Display name of the project |
| `repo` | string | GitHub `owner/name` of the project's public repository |
| `family` | string | `victory` (built on VIctory), `leonida` (built on Leonida) or `independent` |
| `stage` | integer 0–6 | Stage number; 0 means the repository was removed |
| `stage_name` | string | Name of that stage (`Removed` for 0) |
| `fps` | string | Reported frame rate, quoted from the README |
| `test_hardware` | string | Machine the README reports testing on |
| `page` | string or null | Write-up page on gtapcport.org, if one exists |
| `removed` | boolean | `true` if the repository is no longer available |

The live endpoint returns the same projects with a few extra fields (`approach`, `note`, `snap.stars`, `snap.forks`). Stars and forks on the website itself are fetched live from the GitHub API.
