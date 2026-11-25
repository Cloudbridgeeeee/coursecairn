# Proposed AWS architecture

| Service | Role |
|---|---|
| S3 and Lambda | Assessment exports and feedback files, checked on arrival |
| SageMaker AI | Module scoring, gap detection and question analysis |
| Bedrock | Feedback topics and plain-language change notes |
| DynamoDB | Courses, modules, recommendations and the review log |

One AWS account per customer, encrypted at rest and in transit. The public demo calls none of these services.
