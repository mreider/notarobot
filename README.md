# notarobot

Installs the OpenTelemetry Demo on GKE, EKS, and AKS clusters and sends signals to Dynatrace

- Must be logged into a aws, azure, or google cli session
- Must have a current kubectl context

## Grab this repo

```
git clone https://github.com/mreider/notarobot.git
cd notarobot
```

## Set Dynatrace environment variables:

```
export DYNATRACE_ENDPOINT='https://dt.com/api/v2/otlp'
export DYNATRACE_API_TOKEN='..''
```

## Set cloud environment variables:

### Amazon

```
export EKS_CLUSTER_NAME=".."
```

### Azure

```
AKS_CLUSTER_NAME=".."
AKS_RESOURCE_GROUP=".."
```

### Google

```
export GCP_PROJECT_ID='..'
export GKE_CLUSTER_NAME='..'
export GKE_CLUSTER_ZONE='..'
```

## Deploy

Amazon

```
./notarobot aws
```

Azure

```
./notarobot azure
```

Google

```
./notarobot gcp
```

