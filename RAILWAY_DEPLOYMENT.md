# Deploying AppFlowy on Railway

This guide shows how to deploy AppFlowy to Railway as a web application.

## Prerequisites

- A GitHub account
- A Railway.app account
- Fork of the AppFlowy repository

## Steps to Deploy

1. Fork this repository to your GitHub account.

2. Sign in to [Railway](https://railway.app/) and create a new project.

3. Select "Deploy from GitHub repo" and connect your GitHub account.

4. Select your forked AppFlowy repository.

5. Railway will detect the configuration. If asked, select the Dockerfile path as `Dockerfile.railway`.

6. Configure Railway settings:
   - Set the environment variables as needed (if any)
   - The default port is set to 80 in the configuration

7. Deploy the application. Railway will build and deploy your app automatically.

8. Once deployed, Railway will provide you with a URL to access your application.

## Important Notes

- This deployment is for the web version of AppFlowy, which may have some limitations compared to the desktop version.
- The web version uses the browser's local storage for data, so data will be tied to the browser used.
- For production use, you may want to configure SSL/TLS for secure access.

## Troubleshooting

If you encounter issues during deployment:

1. Check the build logs in Railway dashboard for specific error messages.
2. Ensure your repository has the latest version of the configuration files (`railway.toml` and `Dockerfile.railway`).
3. For build failures, you might need to increase the resource allocation in Railway's settings.

## Resources

- [Railway Documentation](https://docs.railway.app/)
- [AppFlowy Documentation](https://appflowy.com/docs)
- [AppFlowy GitHub Repository](https://github.com/AppFlowy-IO/appflowy) 