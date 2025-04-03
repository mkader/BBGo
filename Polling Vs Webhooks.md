* Polling
  1. Polling involves repeatedly checking the external service or endpoint at fixed intervals to retrieve updated information.
  1. It’s like constantly asking, “Do you have something new for me?” even where there might not be any update.
  1. This approach is resource-intensive and inefficient.
  1. Also, you get updates only when you ask for it, thereby missing any real-time information.
  1. However, developers have more control over when and how the data is fetched.

* Webhooks
  1. Webhooks are like having a built-in notification system.
  1. You don’t continuously ask for information.
  1. Instead you create an endpoint in your application server and provide it as a callback to the external service (such as a payment processor or a shipping vendor)
  1. Every time something interesting happens, the external service calls the endpoint and provides the information.
  1. This makes webhooks ideal for dealing with real-time updates because data is pushed to your application as soon as it’s available.

* So, when to use Polling or Webhook?
  1. Polling is a solid option when there is some infrastructural limitation that prevents the use of webhooks. Also, with webhooks there is a risk of missed notifications due to network issues, hence proper retry mechanisms are needed.
  1. Webhooks are recommended for applications that need instant data delivery. Also, webhooks are efficient in terms of resource utilization especially in high throughput environments.

<img src="https://substack-post-media.s3.amazonaws.com/public/images/375dc3ef-ccb8-4627-9b45-67150a0f83f0_1280x1664.gif">
