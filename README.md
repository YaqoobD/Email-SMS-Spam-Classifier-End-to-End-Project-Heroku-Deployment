# Email-SMS-Spam-Classifier-End-to-End-Project-Heroku-Deployment
<script src="https://cdn.jsdelivr.net/npm/mermaid/dist/mermaid.min.js"></script>
```mermaid
graph TB
    A[Input] --> B[Conv2D 7x7, 64 filters]
    B --> C[BatchNorm, ReLU]
    C --> D[Max Pooling 3x3]
    D --> E[Conv2D 1x1, 32 filters]
    E --> F[BatchNorm, ReLU]
    F --> G[Conv2D 3x3, 32 filters]
    G --> H[BatchNorm, ReLU]

