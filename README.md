# Node FRC IP

A lightweight Node.js application for remote IP monitoring. This tool allows you to track and monitor IP addresses efficiently, with the option to run it as a standalone script or as a background service.

## Features
- **Remote IP Monitoring**: Continuously monitor IP addresses for connectivity or changes.
- **Lightweight**: Built with minimal dependencies for fast setup and execution.
- **Flexible Execution**: Run directly via command line or configure as a background service.
- **Cross-Platform**: Compatible with any environment where Node.js is supported.

## Prerequisites
Before you begin, ensure you have the following installed:
- [Node.js](https://nodejs.org/) (v14 or higher recommended)
- [Yarn](https://yarnpkg.com/) (optional, for dependency management)

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/thiagofeijodev/node-frc-ip.git
   ```
2. Navigate to the project directory:
   ```bash
   cd node-frc-ip
   ```
3. Install dependencies:
   ```bash
   yarn install
   ```

## Usage
### Running the Application
To start the application, run:
```bash
yarn start
```

### Running as a Background Service
To set up the application to run as a background service, you can use a process manager like [PM2](https://pm2.keymetrics.io/):
1. Install PM2 globally:
   ```bash
   npm install -g pm2
   ```
2. Start the application with PM2:
   ```bash
   pm2 start index.js --name node-frc-ip
   ```
3. Save the process list to ensure it runs on system startup:
   ```bash
   pm2 save
   ```

### Stopping the Service
To stop the application when running with PM2:
```bash
pm2 stop node-frc-ip
```

## Configuration
The application can be customized via a configuration file (if applicable). Check the `config` directory or refer to the project documentation for details on available settings.

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Commit your changes (`git commit -m 'Add your feature'`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Open a Pull Request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact
For questions or support, feel free to open an issue or contact the maintainer at [thiagofeijodev](https://github.com/thiagofeijodev).

---

© 2025 thiagofeijodev