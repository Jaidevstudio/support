# Community Invitation System

This directory contains the automated GitHub Community Organization invitation system.

## How It Works

1. **Issue Template** (`invitation.yml`): Provides a structured form for users requesting to join the community organization.

2. **Automated Workflow** (`invitation.yml`): Automatically processes invitation requests when issues are labeled with "invite me to the organisation".

## Process Flow

1. User creates a new issue using the invitation template
2. Issue is automatically labeled with "invite me to the organisation"
3. GitHub Actions workflow detects the label and triggers
4. Workflow sends organization invitation to the user
5. Workflow posts confirmation message and closes the issue

## Template Fields

- **Name** (required): User's name
- **Discord Username** (optional): For community Discord access
- **Email** (optional): Contact information
- **Additional Context** (required): Background and motivation for joining

## Troubleshooting

If the automated invitation doesn't work:
- Check that the issue has the correct label: "invite me to the organisation"
- Verify the workflow secrets are properly configured
- Manual invitations can be sent from the organization settings