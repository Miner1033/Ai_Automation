# AI Automation

A collection of AI-powered automation agents and workflows designed to streamline various business and personal tasks using intelligent bots, built with n8n.

## Overview

This repository contains pre-configured n8n workflow JSON files for various AI automation agents that can handle tasks ranging from customer support to social media management, email processing, and business intelligence. Each JSON file can be directly imported into your n8n instance for immediate use.

## Features

### Customer Support & Communication
- **Customer Support Q&A Bot** - Automated responses to common customer inquiries
- **Messenger Agent** - Intelligent messaging automation with character-based responses
- **Email Agent** - Automated email processing and responses
- **Email Marketing** - Automated email campaign management

### Content & Social Media
- **Instagram Post Automation** - Automated social media content creation and posting
- **Multi-agent LinkedIn Posts** - Collaborative content generation for LinkedIn without Tavily integration
- **Webinar Registration** - Automated webinar signup and management

### Business Intelligence
- **Market Research Agent** - Automated market analysis and research compilation
- **Lead Management** - AI-powered lead tracking and qualification using Elete.io
- **Inventory Management** - Automated inventory tracking and alerts

### Productivity & Utilities
- **Daily Weather Bot** - Automated weather updates and notifications
- **Weather to Gmail** - Weather reports delivered directly to your inbox
- **File Backup to Drive** - Automated cloud backup system
- **Gmail Label** - Intelligent email categorization and labeling
- **Motivational Agent** - Daily motivation and inspiration delivery
- **Info Divide by Country** - Geographic data segmentation and organization

### Workflow Automation
- **First AI Powered Workflow** - Template for building custom AI workflows
- **Hablu Bot** - Custom bot configuration

## Getting Started

### Prerequisites
- **n8n** installed (self-hosted or n8n Cloud)
  - [n8n Installation Guide](https://docs.n8n.io/hosting/)
  - [n8n Cloud](https://n8n.io/cloud/)
- Appropriate API keys for integrated services (Gmail, Drive, Elete.io, etc.)
- Basic understanding of n8n workflows

### Installation

1. Clone this repository:
```bash
git clone https://github.com/Miner1033/AI_Automation.git
cd AI_Automation
```

2. Open your n8n instance

3. Import a workflow:
   - Click on **"Workflows"** in the left sidebar
   - Click **"Import from File"** or **"Import from URL"**
   - Select the JSON file you want to use
   - Click **"Import"**

4. Configure credentials:
   - Open the imported workflow
   - Click on nodes that require authentication
   - Add your API keys and credentials
   - Test the connections

5. Activate the workflow:
   - Review the trigger settings
   - Click **"Active"** toggle in the top right
   - Monitor the execution log

### Quick Start with n8n

**Option 1: n8n Cloud**
- Sign up at [n8n.io/cloud](https://n8n.io/cloud/)
- Import workflows directly from this repository
- Configure and activate

**Option 2: Self-Hosted**
```bash
# Using npx
npx n8n

# Using Docker
docker run -it --rm \
  --name n8n \
  -p 5678:5678 \
  -v ~/.n8n:/home/node/.n8n \
  n8nio/n8n
```

Access n8n at `http://localhost:5678`

## Configuration

Each JSON workflow file contains pre-configured n8n nodes and settings. After importing, you'll need to configure:

### Required Credentials
- **Gmail/Google Workspace** - For email automation workflows
- **Google Drive** - For file backup and storage workflows
- **OpenAI/Claude API** - For AI-powered responses and content generation
- **Webhook URLs** - For external integrations
- **Database connections** - If using data storage nodes

### Workflow Customization
1. **Trigger Configuration**: Set up when and how the workflow should start
2. **Node Parameters**: Adjust settings for each node based on your needs
3. **Error Handling**: Configure retry logic and error notifications
4. **Scheduling**: Set up cron expressions for time-based triggers
5. **Testing**: Use n8n's "Execute Workflow" button to test before activation

### Common n8n Nodes Used
- HTTP Request nodes for API calls
- Gmail nodes for email automation
- Google Drive nodes for file operations
- AI nodes (OpenAI, Anthropic Claude) for intelligent responses
- Webhook triggers for external events
- Schedule triggers for time-based automation
- Function nodes for custom JavaScript logic

## Use Cases

- **E-commerce**: Automate customer support, inventory management, and lead tracking
- **Marketing**: Schedule social media posts, manage email campaigns, and conduct market research
- **Productivity**: Automate file backups, email organization, and daily briefings
- **Communication**: Handle messenger queries and email responses automatically

## Contributing

Contributions are welcome! If you have additional automation agents or improvements:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-agent`)
3. Commit your changes (`git commit -m 'Add new automation agent'`)
4. Push to the branch (`git push origin feature/new-agent`)
5. Open a Pull Request

## License

This project is open source. Please check individual files for specific licensing information.

## Support

For issues, questions, or suggestions:
- Open an issue in this GitHub repository
- Check [n8n Community Forum](https://community.n8n.io/)
- Review [n8n Documentation](https://docs.n8n.io/)

## Disclaimer

These n8n automation workflows are provided as-is. Always test workflows thoroughly in a development environment before deploying to production. Ensure compliance with all applicable terms of service for integrated platforms and APIs.

## Resources

- [n8n Official Website](https://n8n.io/)
- [n8n Documentation](https://docs.n8n.io/)
- [n8n Workflow Templates](https://n8n.io/workflows/)
- [n8n Community](https://community.n8n.io/)

---

**Note**: This repository is actively maintained. Check back regularly for new n8n automation workflows and updates.
