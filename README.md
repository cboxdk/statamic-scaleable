# Scaleable Starterpack for Statamic

Welcome to Scaleable – a starter pack for Statamic designed to streamline project setup and prepare your app for cloud-native hosting. This starter pack uses a hybrid database configuration, combining flat files with database storage for optimal performance and flexibility.

## Setup

By initializing your project with this starter pack, your app will be configured to manage both static and dynamic content effectively.

### Architecture and Structure

**Definitions** – The following elements are stored as flat files:

	•	Collections
	•	Asset containers
	•	Navigations
	•	Global sets
	•	Terms
These files should only be managed during local development and deployed as part of the codebase.

**Dynamic Content** – The following elements are stored in the database:

    •	Users
    •	Roles
    •	Entries and entry trees
    •	Navigation trees
    •	Terms
    •	Global set variables
    •	Preview tokens
    •	Forms and form entries
Dynamic content is created and maintained through the control panel on each deployment. This content is not part of the deployment process, enabling definitions to be developed and deployed locally while the actual content remains in the production environment.

## Workflow

	1.	Local Development: Make all changes to structural elements like collections, navigations, and asset containers. These changes will be versioned and deployed alongside the project files.
	2.	Deployment: Deploy definition files to your server. Database content such as user records and entries will remain unchanged and can be accessed via Statamic’s control panel in the cloud-native setup.
	3.	Content Management: After deployment, all content updates should be done directly through the control panel in each deployment environment. This ensures that content changes are only updated in the database and will not be overwritten by future deployments.

## Installation

To get started, clone this repository and follow the standard Statamic installation procedures. Follow the setup instructions to ensure the hybrid configuration operates as intended.

## Benefits of Scaleable Starter Pack

    •	Efficient Cloud-Native Hosting: The combination of flat files and database content allows you to version structural and definition files without affecting dynamic content.
    •	Flexible Setup: Manage structural changes via deployment, while keeping content flexible and manageable within each environment.
    •	Scalable and Reliable: Ideal for production environments where version control and dynamic content management are both required.