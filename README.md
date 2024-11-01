* System Design - https://bytebytego.com/courses/system-design-interview/scale-from-zero-to-millions-of-users
* Video tutorials for modern ideas and open source tools - https://calmcode.io/
* Data Science - https://aigents.co/learn

## Big Data Pipeline Cheatsheet for AWS, Azure, and Google Cloud
* Each platform offers a comprehensive suite of services that cover the entire lifecycle:
    1. Ingestion: Collecting data from various sources
    1. Data Lake: Storing raw data
    1. Computation: Processing and analyzing data
    1. Data Warehouse: Storing structured data
    1. Presentation: Visualizing and reporting insights

## The Software Development Life Cycle (SDLC) is a framework that outlines the process of developing software in a systematic way. Here are some of the most common ones:
* Waterfall Model:
    1. A linear and sequential approach.
    1. Divides the project into distinct phases: Requirements, Design, Implementation, Verification, and Maintenance.

* Agile Model:
    1. Development is done in small, manageable increments called sprints.
    1. Common Agile methodologies include Scrum, Kanban, and Extreme Programming (XP).

* V-Model (Validation and Verification Model):
    1. An extension of the Waterfall model.
    2. Each development phase is associated with a testing phase, forming a V shape.

* Iterative Model:
    1. Focuses on building a system incrementally.
    1. Each iteration builds upon the previous one until the final product is achieved.

* Spiral Model:
    1. Combines iterative development with systematic aspects of the Waterfall model.
    1. Each cycle involves planning, risk analysis, engineering, and evaluation.

* Big Bang Model:
    1. All coding is done with minimal planning, and the entire software is integrated and tested at once.

* RAD Model (Rapid Application Development):
    1. Emphasizes rapid prototyping and quick feedback.
    1. Focuses on quick development and delivery.

* Incremental Model:
    1. The product is designed, implemented, and tested incrementally until the product is finished.
 
 ## There are multiple stages in a Terraform workflow:
* Write Infrastructure as Code
    1. Define resources, providers, and configurations in Terraform configuration files.
    1. Use variables, modules, and functions to make the code reusable and maintainable.
    1. Integrate with Terraform community registries for ready-to-use modules.

* Terraform Plan
    1. Preview the changes Terraform will make to the infrastructure by running “terraform plan”. It can be triggered as part of a CI/CD pipeline.
    1. Terraform compares the desired state defined in the configuration file with the current state in the state file.

* Terraform Apply
    1. Run “terraform apply” to create, update, or delete resources based on the plan.
    1. Terraform makes API calls to the specified providers (AWS, Azure, GCP, Kubernetes, etc) to provision the resources.
    1. The state file is updated to reflect the new state of the infrastructure.

* Infrastructure Ready
    1. Terraform state file acts as a single source of truth for the current state of the infrastructure.
    1. State file enables version control and collaboration between team members for future changes.
