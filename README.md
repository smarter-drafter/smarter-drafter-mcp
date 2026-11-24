# Smarter Drafter for Google Antigravity

Draft client-ready legal documents from your firm's approved Smarter Drafter templates, without leaving Antigravity.

You describe the document you need. The agent finds the right Smarter Drafter form, asks only the questions the form needs, and sends your answers to Smarter Drafter. Smarter Drafter builds the document from your firm's template and returns it as PDF or DOCX. The AI does not write the document text, so there are no invented clauses or citations.

## Before you start

- You need a Smarter Drafter account.
- Your firm must have at least one published form that you can access.

## Set up

1. Install the plugin.
2. Start a task that uses Smarter Drafter, for example "Find the Smarter Drafter form for a letter of engagement".
3. When Antigravity asks, sign in with your Smarter Drafter account and approve the permissions.

### Region

The plugin connects to the Australian server (`https://mcp.smarterdrafter.com`) by default. This server is for all customers outside the UK and EU.

UK and EU customers use `https://mcp.smarterdrafter.co.uk`. In the plugin's MCP settings, turn on the `uk` server and turn off the `au` server.

## Tools

| Tool | What it does |
| --- | --- |
| `search_forms` | Finds published forms in your Smarter Drafter account by name or description. |
| `get_fields_by_form` | Gets the fields of a form: types, validation rules, options and repeating sections. |
| `create_submission` | Creates a submission with your answers. A draft can be finished later. |
| `update_submission_answer` | Changes one answer in a submission. |
| `attach_submission_file` | Adds a file from a public URL to a file field in a draft submission. |
| `submit_submission` | Completes a draft submission and starts document generation. |
| `get_submission_generated_documents_url` | Returns short-lived download links for the generated documents. |
| `get_submission_generated_documents` | Returns the generated documents as files, for when the links cannot be downloaded. |

## Example workflows

- **Draft a document:** "Draft an NDA for John Wickham using our firm's Smarter Drafter template." The agent finds the NDA form, asks for the missing details, generates the document and gives you the download links.
- **Hand off a long form:** "Start a lease agreement for 12 Smith Street and let me finish the rest in Smarter Drafter." The agent fills what it knows and gives you a link to complete the other fields in Smarter Drafter.
- **Check what a form needs:** "Which details does our employment agreement form need?"

## Permissions and security

- Sign-in uses OAuth with PKCE. You see only the forms you can access in Smarter Drafter.
- Every action is recorded against your own user.
- Completing a submission can start emails, webhooks or uploads that your firm set up on the form.

Full details: [Smarter Drafter MCP server documentation](https://developers.smarterdrafter.com/reference/mcp-server).

## Support

- Email: [support@smarterdrafter.com](mailto:support@smarterdrafter.com)
- Support request: [knowledge.smarterdrafter.com](https://knowledge.smarterdrafter.com/contact-us/general-support-request)
- Privacy policy: [smarterdrafter.com/privacy-policy](https://smarterdrafter.com/privacy-policy/)
