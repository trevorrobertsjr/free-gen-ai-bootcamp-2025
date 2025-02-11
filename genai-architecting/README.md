# Architecture
## Functional Requirements

The system must be capable of scaling to meet peak student load and deactivate scaled out resources during low traffic periods.

The system must have low latency to end users.

## Assumptions

The cloud provider has sufficient quantity of powerful compute resources to meet peak load.

A single instance will be sufficient for an initial soft launch.

Due to predetermined structure of the course curriculum, cache hits will be high with less traffic expected to hit the model directly.

## Data Strategy

Specialized data will be licensed and stored in the vector database.

The data will be stored using sparse encoding when possible to improve performance.