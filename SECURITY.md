# Security policy

## Reporting a vulnerability

Do not open a public issue with exploit details, credentials, personal data, or sensitive execution logs.

Report a suspected vulnerability privately through GitHub: open the repository's **Security** tab and select **Report a vulnerability**. Reports are visible only to the repository owner.

## Using this workflow safely

- **Credentials** — the exported workflow contains no credentials. Connect your own OpenAI, Gmail, and Google Sheets credentials inside n8n; never paste API keys into node parameters or prompts.
- **Public intake form** — the *Brief Intake Form* has no authentication. Anyone with its production URL can submit briefs, and each submission spends your OpenAI credits. Enable **Basic Auth** on that node before activating the workflow.
- **Email recipients** — replace the `*@example.com` placeholders in *Config — Brand + Brief* with addresses you control. Review emails carry approval links: anyone who receives them can approve or reject content.
- **Audit sheet** — the Google Sheet stores generated content and reviewer feedback. Share it only with the people who need it.
- **Re-exporting** — n8n exports keep credential IDs, webhook IDs, and instance metadata. Remove them before sharing your own copy of the workflow.
