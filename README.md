## Background

This folder contains a simple Helm chart which will deploy a containerized application.  This application will start an HTTP listener on a port and respond to a `GET` request with a message.  If the application has been properly deployed, the message will include a code indicating success. This code should be provided back to the interviewer as proof of successful completion of the test.

# Instructions

Contents of the chart are as follows:

```
my-helm-chart
├── Chart.yaml
├── README.md
├── templates
│   ├── deployment.yaml
│   └── service.yaml
└── values.yaml
```

You will need to deploy this chart to a Kubernetes environment (e.g. KinD or other testing environment you have available).  In addition, there is a small bug in the chart that will need to be debugged and fixed in order for the chart to properly install. Once you've successfully deployed the chart, please visit the service on the exposed port and provide the success code that is returned.