
### Editing the `.yaml` File

You can edit the `.yaml` file using one of the following methods:

1. **Online**: Use the [Swagger Editor](https://editor.swagger.io/).
2. **Locally**: Clone the Swagger Editor repository and run it locally. Instructions are available [here](https://github.com/swagger-api/swagger-editor).

**Importing a File:** Before starting to edit, you can import your `.yaml` file into the editor. Go to the **File** tab and click **Import File** to load your existing YAML.

**Exporting a File:** After finishing your edits, export the updated `.yaml` file. Go to the **File** tab and click **Save as YAML**. This file will be used to generate the HTML documentation.

---

### Generating the `.html` File

To create an HTML version of your API documentation:

1. **Install Node.js**: Ensure you have [Node.js](https://nodejs.org/en) installed on your machine.

2. **Install Redocly CLI**: Check if Redocly CLI is installed by running:
   ```bash
   redocly --version
   ```
   If it's not installed, run:
   ```bash
   npm install -g @redocly/cli
   ```
3. **Build the Documentation**: Run the following command to generate the HTML file from your exported `.yaml` file:
   ```bash
   redocly build-docs path/to/your/openapi.yaml -o api-documentation.html
   ```