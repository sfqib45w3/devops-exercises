# CI/CD Exercises

## Questions & Concepts

#### What is CI/CD?
Continuous Integration (CI) is the practice of automating the integration of code changes from multiple contributors into a shared repository. Continuous Delivery/Deployment (CD) automates the release process so that software can be deployed to production quickly and reliably.

#### What is the difference between Continuous Delivery and Continuous Deployment?
* **Continuous Delivery**: Code changes are automatically built, tested, and prepared for release to production. Deployment to production requires manual approval.
* **Continuous Deployment**: Every change that passes all stages of the pipeline is automatically deployed directly to production without manual intervention.

#### What are typical stages in a CI/CD pipeline?
1. **Source**: Triggering the pipeline on code commits or pull requests.
2. **Build**: Compiling code, building container images, and creating artifacts.
3. **Test**: Running unit, integration, linting, and security vulnerability scans.
4. **Deploy**: Publishing artifacts to staging/production environments.
5. **Observe & Verify**: Running automated smoke tests and health checks to confirm deployment stability.

#### What is Blue-Green Deployment?
A technique that reduces downtime by running two identical environments (Blue and Green). Only one environment serves live traffic at a time; updates are deployed to the idle environment before switching traffic.

#### What is Canary Deployment?
A deployment strategy where a new software version is incrementally rolled out to a small percentage of users before deploying to the entire user base.