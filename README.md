# Simple Frontend Project

This is a simple static website built with HTML, CSS, and JavaScript.

## Getting Started

1. Clone the repository.
2. Open `index.html` in your browser.

## CI/CD

This project includes a GitHub Actions workflow for CI/CD deployment to Azure VM at 172.179.1.229.

To set up deployment:
1. In your GitHub repository, go to Settings > Secrets and variables > Actions.
2. Add the following secrets:
   - `AZURE_VM_HOST`: 172.179.1.229
   - `AZURE_VM_USER`: your VM username
   - `AZURE_VM_SSH_KEY`: your private SSH key
3. Update the workflow file `.github/workflows/deploy.yml` with the correct path on your VM.

## Deployment

The CI/CD pipeline will automatically deploy to your Azure VM on push to main branch.