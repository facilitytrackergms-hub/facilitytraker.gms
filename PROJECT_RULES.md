Project Rules

One Door Method:
- A door is the shared identity for a room, area, location, equipment item, or future work object.
- Categories are access points, not separate identities.
- Weekly Room is the base weekly schedule.
- Daily Room is an extra access label from room_settings.isDaily.
- A Daily-labeled Weekly Room must not become a separate Daily Room identity.

Data rules:
- Keep existing Firebase project and Firestore collection names.
- Do not rename collections such as areas, tasks, room_settings, task_area_status, task_history, issue_logs, issue_reasons, employees, schedules, or settings.
- Use shared roomKey identity for room-based Weekly/Daily behavior.
- Preserve true Daily Room-only records when no Weekly Room base exists.

Development rules:
- Keep the current app working while improving one area at a time.
- Avoid changing save/delete/reassignment behavior without a specific test.
- Avoid browser alert/confirm/prompt in new UI work when an in-app modal can be used.
- Keep mobile-first layouts and large readable controls.
