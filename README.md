# Receipt Generator

A simple web application for generating receipts. This application is hosted on AWS Amplify and can be accessed at [https://main.d25p4rrogwkjec.amplifyapp.com/](https://main.d25p4rrogwkjec.amplifyapp.com/).

## Hosting on AWS Amplify: Step-by-Step Guide

### Prerequisites
- An AWS account
- A GitHub, GitLab, Bitbucket, or AWS CodeCommit repository with your receipt generator code
- Basic knowledge of Git

### Step 1: Prepare Your Application
1. Ensure your application is working correctly locally
2. Make sure your repository includes:
   - HTML files (index.html, nav.html)
   - Any CSS and JavaScript files
   - A proper directory structure

### Step 2: Push Your Code to a Git Repository
1. Initialize Git in your project folder (if not already done):
   ```bash
   git init
   ```
2. Add your files to Git:
   ```bash
   git add .
   ```
3. Commit your changes:
   ```bash
   git commit -m "Initial commit"
   ```
4. Create a repository on GitHub/GitLab/Bitbucket
5. Add the remote repository:
   ```bash
   git remote add origin <your-repository-url>
   ```
6. Push your code:
   ```bash
   git push -u origin main
   ```

### Step 3: Deploy with AWS Amplify
1. Sign in to the [AWS Management Console](https://aws.amazon.com/console/)
2. Search for "Amplify" in the services search bar and select it
3. Click "New app" and select "Host web app"
4. Choose your Git provider (GitHub, GitLab, Bitbucket, or AWS CodeCommit)
5. Authorize AWS Amplify to access your repositories
6. Select the repository containing your receipt generator
7. Select the branch you want to deploy (e.g., main)
8. Configure build settings:
   - For a simple static site, the default settings should work
   - If you have specific build commands, you can add them here
9. Review your settings and click "Save and deploy"

### Step 4: Monitor the Deployment
1. Amplify will start building and deploying your application
2. You can monitor the progress in the Amplify Console
3. Once deployment is complete, Amplify will provide a URL to access your application

### Step 5: Custom Domain (Optional)
1. In the Amplify Console, go to "Domain management"
2. Click "Add domain"
3. Enter your domain name and click "Configure domain"
4. Follow the instructions to verify domain ownership and set up DNS records
5. Wait for DNS propagation (can take up to 48 hours)

### Step 6: Continuous Deployment
AWS Amplify automatically sets up continuous deployment. When you push changes to your repository:
1. Amplify detects the changes
2. Builds and deploys the updated application
3. Makes the new version available at your Amplify URL

## Troubleshooting
- If your deployment fails, check the build logs in the Amplify Console
- Ensure all dependencies are properly included in your repository
- Verify that your application works locally before deploying

## Additional Resources
- [AWS Amplify Documentation](https://docs.aws.amazon.com/amplify/)
- [AWS Amplify Console User Guide](https://docs.aws.amazon.com/amplify/latest/userguide/welcome.html)