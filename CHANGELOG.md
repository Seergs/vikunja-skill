# Changelog

All notable changes to this skill will be documented here.
Versioning follows [Semantic Versioning](https://semver.org/).

## [1.0.2] - 2026-04-05

### Fixed
- Correct clawhub installation command

### Added
- Tasks: task relations

## [1.0.1] - 2026-03-31

### Fixed
- Declare VIKUNJA_BASE_URL and VIKUNJA_API_TOKEN in skill metadata
- Add homepage to skill metadata for provenance

## [1.0.0] - 2026-03-31

### Added
- Initial release
- Projects: list, get, create
- Tasks: list (all + by project), get, create, update, mark done, delete
- Labels: list, create, add to task, remove from task
- Assignees: list, add, remove
- Reminders: absolute datetime and relative-to-task-date
- API token authentication via `VIKUNJA_API_TOKEN` env var
- Configurable base URL via `VIKUNJA_BASE_URL` env var
- Tested against Vikunja 0.24.x
