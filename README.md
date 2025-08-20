Smart Substitute Recommender
Project Overview

This project is a modern e-commerce application that demonstrates a smarter way to handle out-of-stock products. Instead of simply showing a "sold out" message, our system uses AI-powered semantic search to recommend the most suitable alternatives from the product catalog.

The core of this application is a BigQuery-powered back-end that leverages vector embeddings. These are a way of representing text as numerical vectors, allowing us to find products that are not just in the same category but are also functionally and stylistically similar.

This project is an excellent demonstration of how to integrate cutting-edge AI features from Google Cloud into a practical, real-world application to improve user experience and recover lost sales.
Key Features

    Intelligent Recommendations: Go beyond simple keyword or category matching to provide genuinely useful product substitutes.

    BigQuery Integration: Use BigQuery ML to transform product descriptions into rich vector embeddings.

    Efficient Vector Search: Employ BigQuery's built-in VECTOR_SEARCH function for blazing-fast similarity lookups.

    Scalable Architecture: Built with a scalable back-end and a modern front-end ready for production use.

    Enhanced E-commerce: A practical solution to a common business problem, demonstrating a direct return on investment from AI.

Architecture

The system is split into two main components:

    Back-End (/backend):

        Handles all communication with Google Cloud services, specifically BigQuery.

        Exposes a REST API endpoint that takes a product_id and returns a list of recommended substitutes.

        Languages/Frameworks: Python (Flask/Django) or Node.js (Express).

    Front-End (/frontend):

        A single-page application that simulates a product page.

        Displays product information and fetches substitute recommendations from the back-end API when an item is marked as out of stock.

        Languages/Frameworks: React, Vue.js.

The project relies on a BigQuery dataset that stores product information and their corresponding vector embeddings. This data is the foundation of the recommendation engine.
Getting Started
Prerequisites

    A Google Cloud account with an active project.

    The gcloud CLI installed and authenticated.

    BigQuery API and BigQuery Connection API enabled.

    A BigQuery connection to Vertex AI for the embedding model.

Installation

    Clone the repository:
    git clone https://github.com/your-username/your-repo-name.git
    cd your-repo-name

    Back-End Setup:
    cd backend
    Follow the specific instructions in the backend/README.md for your chosen language (Python or Node.js).

    Front-End Setup:
    cd ../frontend
    Follow the specific instructions in the frontend/README.md for your chosen framework (React or Vue.js).

    BigQuery Setup:

        Run the provided SQL scripts in the sql/ directory to create the necessary tables and vector index in your BigQuery project.

        This will handle the data ingestion, embedding generation, and index creation for the product catalog.

Contributing

We welcome contributions! Please see our CONTRIBUTING.md file for guidelines on how to submit pull requests, report issues, and help improve the project.
License

This project is licensed under the MIT License.
