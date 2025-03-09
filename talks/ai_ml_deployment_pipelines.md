# Deploying AI/ML Pipelines at Crexi

Isaac Smothers & Xpaul Vigil

[Deploying AI/ML Pipelines](https://www.socallinuxexpo.org/scale/22x/presentations/deploying-aiml-pipelines-crexi)

- Work with our other favorite scale speaker, James Healy-Mirkovich
- Introducing self-service infrastructure, with AI helper. DEMO1!
- Generates YAML with "depends on" attributes for chains of models

## Implementation details
- Pulumi IaC (like terraform), AWS, OTel/Datadog, GitHub Actions
- Inputs (SNS, S3 Triggers) -> Lambda -> Sagemaker -> Outputs (e.g. SNS, Kinesis Firehose)
- Can combine smaller pipeline units into mega-pipelines
- ✨Observability✨ with DataDog

## DEMO2!

- Ask Crexi self-service GPT to create buckets that pull from csv files and create lambdas with correct dependencies
- Best practices are baked-in with yaml definitions
- Provides good template for starting off with new services
- It can tell you which services it does and does not support

## Questions
- Pulumi takes yaml and does all the things with it. GitHub Actions just kicks it off
- Use OpenAI to build yamls for developers
- Pinned to exact versions of Pulumi and update as needed (with tests), and Pulumi itself has idea of dependencies for individual services
- Repo setup requires a ticket (for GitHub Action auth) but then kicks off Pulumi
