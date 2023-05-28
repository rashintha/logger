# Logger

![Go](https://img.shields.io/badge/GO-00ADD8?logo=go&logoColor=white&style=for-the-badge)

## Introduction

Logger is a basic logging library that could be used in API logging and any other code where terminal and file logging is required.

## Getting Started

### Prerequisites

- **[Go](https://go.dev/)**

### Get the Logger

Simply run the following command to get the logger package.

```bash
go get github.com/rashintha/logger
```

### Basic Usage

Logger will create `log/log.log` file in your app's root directory and will print the log to your terminal as well as to the log file.

```go
package main

import "github.com/rashintha/logger"

func main() {
	// Default log
	logger.Defaultln("Default log line")
	logger.Defaultf("Default log line with %v", "parameters")

	// Information log
	logger.Infoln("Information log line")
	logger.Infof("Information log line with %v", "parameters")

	// Warning log
	logger.Warningln("Warning log line")
	logger.Warningf("Warning log line with %v", "variables")

	// Error log
	logger.Errorln("Error log line")
	logger.Errorf("Error log line with %v", "parameters")
	logger.ErrorFatal("Fatal error log line")
	logger.ErrorFatalf("Fatal error log line with %v", "parameters")	
}

```

## License

Logger is released under Apache-2.0 license. Please read [LICENSE](LICENSE) for more information.

## Contributing

I always appreciate help from the community to develop. Please send me an email to mail@rashintha.com to get started!