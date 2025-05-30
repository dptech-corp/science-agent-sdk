# Science Agent SDK

This is DP Tech's Science Agent SDK, providing a command-line tool `dp-agent` for managing scientific computing tasks.

## Installation

### Linux/Mac

```bash
pip install science-agent-sdk --upgrade
```

### Windows

In PowerShell, run:

```powershell
pip install science-agent-sdk --upgrade
```

## Usage

After installation, you can use the following commands:

### Fetch Scaffolding

```bash
dp-agent fetch scaffolding --type=cloud/calculation/device
```

### Fetch Configuration

```bash
dp-agent fetch config
```

This command downloads the .env file and replaces dynamic variables such as MQTT_DEVICE_ID.
Note: For security reasons, this feature is only available in internal network environments. Other environments require manual configuration.

### Run Lab Environment

```bash
dp-agent run tool device
```

### Run Cloud Environment

```bash
dp-agent run tool cloud
```
### Run Calculation Environment

```bash
dp-agent run tool calculation
```

### Run Agent

```bash
dp-agent run agent
```

### Debug Cloud Environment

```bash
dp-agent run debug
```

## Development Notes

This SDK provides a client-server architecture for submitting and managing scientific computing tasks. For detailed API documentation, please refer to the comments in the code.
