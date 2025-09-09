* Use official images - This ensures security, reliability, and regular updates.
* Use a specific image version - The default latest tag is unpredictable and causes unexpected behavior.
* Multi-Stage builds - Reduces final image size by excluding build tools and dependencies.
* Use .dockerignore - Excludes unnecessary files, speeds up builds, and reduces image size.
* Use the least privileged user - Enhances security by limiting container privileges.
* Use environment variables - Increases flexibility and portability across different environments.
* Order matters for caching - Order your steps from least to most frequently changing to optimize caching.
* Label your images - It improves organization and helps with image management.
* Scan images - Find security vulnerabilities before they become bigger problems.

<img src="https://github.com/mkader/BBGo/blob/main/9%20Docker%20Best%20Practices.png">
