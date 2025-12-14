# Sample documentation timeline

This example shows how a documentation timeline might be structured for a medium-complexity feature with a 12-week development cycle.

## Timeline diagram

This diagram illustrates the key milestones and their temporal relationships throughout the documentation lifecycle.

```
Planning period starts
│
├─ Week 1: Parent initiative created
│           Documentation request created
│           Documentation plan completed
│           Writer assigned
│
├─ Week 2-10: Development phase
│
├─ Code complete - 2 weeks: Notification to docs team
│
├─ Code complete
│
├─ Launch - Lead time: Reviewable draft due
│  │
│  │  Low complexity:    Launch - 1 week
│  │  Medium complexity: Launch - 2 weeks
│  │  High complexity:   Launch - 4 weeks
│  │
│  └─ Writer review period
│
├─ Launch - 2 weeks: Documentation cut-off
│  │
│  └─ Final changes window closes
│
└─ Launch
```

## Milestone descriptions

### Planning period starts (Week 0)

The planning period begins when the product team starts defining the scope and timeline for the upcoming work. This marks the beginning of the documentation process.

### Week 1: Initial setup

Four critical activities happen in the first week:

- **Parent initiative created.** Product manager creates the parent initiative in the project tracker.
- **Documentation request created.** Product manager creates the documentation request as a child of the parent initiative.
- **Documentation plan completed.** Product manager fills out the documentation plan template with all required information.
- **Writer assigned.** Documentation lead assigns a writer to the project based on the completed plan.

### Week 2-10: Development phase

The team builds the feature. The writer monitors progress and stays informed about changes to the feature scope or implementation.

### Notification to docs team (Week 8, Code complete - 2 weeks)

Two weeks before code complete, the product manager notifies the docs team of the upcoming code complete date. This allows the writer to plan their review work.

### Code complete (Week 10)

The feature implementation is complete and ready for testing. Code may still change during the review period, but major functionality is in place.

### Reviewable draft due (Week 10, Launch - 2 weeks)

The engineer or product manager provides a reviewable draft to the writer. In this medium-complexity example, the draft is due two weeks before launch.

The writer reviews the draft and provides feedback. The review period continues until the documentation cut-off.

### Documentation cut-off (Week 10, Launch - 2 weeks)

Two weeks before launch, the documentation enters final preparation. No new changes are accepted except for critical corrections.

### Launch (Week 12)

The feature ships and documentation publishes.

## Timeline variations for this example

### If complexity was low

For a low-complexity version of this feature, the reviewable draft would be due in week 11 (launch - 1 week) instead of week 10. The development phase might also be shorter (8 weeks instead of 10).

### If complexity was high

For a high-complexity version, the reviewable draft would be due in week 8 (launch - 4 weeks), requiring earlier code stabilization. The development phase might be longer (16+ weeks).

### If the planning period was compressed

If planning started in week 3 instead of week 1, the writer might not be assigned until week 4. This would require either:

- Extending the launch date to maintain quality
- Reducing documentation scope
- Accepting higher risk in the documentation process
