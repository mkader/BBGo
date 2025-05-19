1. Multi-Service Deployment
  * In this model, we deploy new changes to multiple services simultaneously.
  * This approach is easy to implement. But since all the services are upgraded at the same time, it is hard to manage and test dependencies.
  * It’s also hard to rollback safely.

1. Blue-Green Deployment
  * With blue-green deployment, we have two identical environments: one is staging (blue) and the other is production (green).
  * The staging environment is one version ahead of production.
  * Once testing is done in the staging environment, user traffic is switched to the staging environment, and the staging becomes the production.
  * This deployment strategy is simple to perform rollback, but having two identical production quality environments could be expensive.

1. Canary Deployment
  * A canary deployment upgrades services gradually, each time to a subset of users.
  * It is cheaper than blue-green deployment and easy to perform rollback. However, since there is no staging environment, we have to test on production.
  * This process is more complicated because we need to monitor the canary while gradually migrating more and more users away from the old version.

1. A/B Test
  * In the A/B test, different versions of services run in production simultaneously.
  * Each version runs an “experiment” for a subset of users.
  * A/B test is a cheap method to test new features in production.
  * We need to control the deployment process in case some features are pushed to users by accident.

<img src="https://substack-post-media.s3.amazonaws.com/public/images/8a4a708d-20f3-47d9-92a0-ac826585711e_1280x1664.gif">
