# Communishield Deployment Repository

## Overview

The `communishield-deployment` repository contains the Docker Compose configuration for the backend, frontend, and reverse proxy.

## Running the Application

1. Clone the deployment repository and initialize submodules:

   ```bash
   git clone --recurse-submodules git@github.com:communishield/communishield-deployment.git
   ```

2. Navigate to the cloned directory:

   ```bash
   cd communishield-deployment
   ```

3. Run the Docker Compose:

   ```bash
   docker-compose up
   ```

   This command will build and start all the necessary services:

   - The reverse proxy will be accessible on ports 80 (HTTP) and 443 (HTTPS).
   - The backend, Postgres, and frontend services will be set up according to their respective Docker Compose configurations in the submodules.

### Updating Submodules

To update the submodules to the latest versions:

```bash
git submodule update --remote
```

## License

The Communishield Deployment Repository, like the individual backend and frontend components, is open-source software licensed under the AGPL-3.0. For more information, see the [LICENSE](https://github.com/communishield/communishield-deployment/blob/main/LICENSE) in the repository.
