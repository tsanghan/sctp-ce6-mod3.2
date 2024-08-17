# sctp-ce6-mod3.2

### 1. What is GitHub Authentication?

GitHub Authentication is the process of verifying your identity when accessing GitHub resources like repositories, issues, and pull requests. Authentication is crucial for maintaining security and ensuring that only authorized users can access or modify a repository. It can be implemented using various methods, allowing users to choose the one that best fits their needs.

**Methods of GitHub Authentication:**

1. **Password Authentication:**
   - *Deprecated*: Password-based authentication for Git operations has been removed in favor of more secure methods.

2. **Personal Access Tokens (PAT):**
   - A personal access token works like a password for GitHub. It grants access to specific repositories and scopes that you define. This is more secure than using a password because you can restrict the scope of access and revoke the token if it’s compromised.

3. **SSH Keys:**
   - SSH keys are cryptographic keys that provide a secure way to authenticate with GitHub without using a password. You generate a public/private key pair, upload the public key to GitHub, and use the private key on your local machine to authenticate.

4. **OAuth Tokens:**
   - OAuth tokens allow third-party applications to interact with your GitHub account securely. When you authenticate using OAuth, you’re granting an application specific permissions to act on your behalf.

5. **GitHub App Installation Access Tokens:**
   - GitHub Apps authenticate using installation access tokens, which are generated for specific GitHub App installations. These tokens provide the GitHub App with a temporary and limited ability to act on your behalf.

6. **Web Authentication via Browser:**
   - When accessing GitHub via the web interface, authentication is typically done using a combination of username/password and two-factor authentication (2FA). You can also use Single Sign-On (SSO) for enterprise accounts.
