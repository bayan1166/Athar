# MultiSensor-Home1 Dataset Audit

## Dataset Summary
- Training records: 355
- Testing records: 150
- All labels records: 511
- Training annotated events: 946
- Activity classes: 16
- Camera views per record: 5

## Consistency Check
- Unique train/test records: 505
- Unique all_labels records: 511
- Shared records: 391
- Only in all_labels: 120
- Only in train/test: 114
- Annotation mismatches on shared records: 0

## Observations
- Train/test use CAM6-CAM10 naming.
- all_labels uses View1-View5 naming.
- All training events have channel = 0.

## Decisions
- Preserve all original JSON files.
- Use train.json and test.json as initial splits.
- Do not merge all_labels into train/test.
- Verify filenames and timestamps against actual videos.

## Status
JSON audit completed.
Video inspection pending.