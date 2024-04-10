# NetCharger

NetCharger is a lightweight, powerful TCP stress testing tool designed to evaluate the performance and resilience of TCP servers by establishing a large number of connections simultaneously. It operates in two modes: a **Server Mode** for listening and responding to incoming TCP connections, and a **Stress Test Mode** for initiating connections to a specified server.

## Features

- **Server Mode**: Runs a simple TCP server that listens on a configurable port and responds with a predefined message to each incoming connection.
- **Stress Test Mode**: Simultaneously initiates thousands of TCP connections to test the throughput and handling capacity of a TCP server.

## Getting Started

### Prerequisites

- Go 1.17 or later

### Installation

Clone the repository to your local machine:

```
git clone https://github.com/jash2105/NetCharger.git
```

Navigate to the project directory:

```
cd NetCharger
```

### Usage

To start the tool in **Server Mode**:

```
go run net_charger.go listen
```

To start the tool in **Stress Test Mode** and connect to specified host(s):

```
go run net_charger.go <host1> <host2> ...
```

Replace `<host1>`, `<host2>`, etc., with the actual IP addresses or hostnames of the servers you want to test.

### Building the Project

To build the project for deployment:

```
go build -o net_charger net_charger.go
```

This will generate an executable file named `net_charger`.




