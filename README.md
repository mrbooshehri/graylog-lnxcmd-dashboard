# Graylog Content Pack for Syslog Log Analysis

This content pack is designed to enhance Graylog's syslog log analysis capabilities by parsing logs with a custom Grok pattern and visualizing issued commands per user on all hosts as a pie chart. It's tailored for environments where understanding user activity and command usage is crucial for system administration and security monitoring.

## Features

- **Log Parsing**: Utilizes a custom Grok pattern to parse syslog logs, extracting relevant information such as user, shell PID, and command executed.
- **Visualization**: Generates a pie chart demonstrating the issued command per user on all hosts, providing a clear overview of user activity.
- **Customizable**: Allows for easy customization of the Grok pattern and visualization settings to fit specific logging formats and visualization needs.

## Installation

1. **Download the Content Pack**: Download the content pack package from the provided link or repository.
2. **Upload to Graylog**: Log in to your Graylog instance, navigate to the Content Packs section, and upload the downloaded package.
3. **Activate the Content Pack**: After uploading, activate the content pack to start processing logs with the custom Grok pattern and generating visualizations.

## Configuration

### Grok Pattern

- The content pack comes with a predefined Grok pattern tailored for the log format `User: [ devops ] Shell PID: [22072] command: ls`.
- If your logs have a different format, you can customize the Grok pattern in the content pack's configuration.

### Visualization Settings

- The pie chart visualization is configured to display the issued command per user on all hosts.
- You can adjust the visualization settings, such as the time range and refresh interval, directly from the Kibana dashboard.

## Usage

- Once the content pack is activated and configured, Graylog will start processing syslog logs according to the custom Grok pattern.
- The pie chart visualization will automatically update, reflecting the issued command per user on all hosts based on the processed logs.

## Troubleshooting

- If logs are not being processed as expected, check the Grok pattern for accuracy and ensure your syslog server is correctly configured to send logs to Graylog.
- For visualization issues, verify the Kibana dashboard settings and ensure the content pack's visualization is correctly configured.

## Contributing

Contributions to improve the content pack, such as adding support for additional log formats or enhancing visualization options, are welcome. Please submit pull requests or issues through the repository.

## License

This content pack is licensed under the MIT License. See the LICENSE file for details.

