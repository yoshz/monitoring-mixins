# Monitoring Mixins

Simple jsonnet bundle to generate monitoring mixins for Prometheus and Kubernetes

## Prerequisites

```bash
# install system dependencies
sudo apt install golang-1.14-go

# install jsonnet
go get github.com/google/go-jsonnet/cmd/jsonnet
go get github.com/google/go-jsonnet/cmd/jsonnetfmt

# install jsonnet-bundler
go get github.com/jsonnet-bundler/jsonnet-bundler/cmd/jb

# install promtool
go get github.com/prometheus/prometheus/cmd/promtool
```

## Installation

```bash
# install dependencies
jb install
```

## Usage

```bash
# make all rules, alerts and dashboards, lint the files and test with promtool
make

# make dashboards
make dashboards_out

# make alerts
make prometheus_alerts.yaml

# make rules
make prometheus_rules.yaml
```