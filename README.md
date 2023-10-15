/**
 * Represents a website about volcanoes and awareness.
 */
class VolcanoWebsite {
    /**
     * Constructor for the VolcanoWebsite class.
     *
     * @param {string} title - The title of the website.
     * @param {string} description - The description of the website.
     */
    constructor(title, description) {
        /** @private */
        this.title = title;

        /** @private */
        this.description = description;
    }

    /**
     * Getter method to retrieve the title of the website.
     *
     * @returns {string} The title of the website.
     */
    getTitle() {
        return this.title;
    }

    /**
     * Getter method to retrieve the description of the website.
     *
     * @returns {string} The description of the website.
     */
    getDescription() {
        return this.description;
    }

    /**
     * Generates the HTML content for the website.
     *
     * @returns {string} The HTML content of the website.
     */
    generateWebsiteContent() {
        return `
            <html>
                <head>
                    <title>${this.title}</title>
                </head>
                <body>
                    <h1>${this.title}</h1>
                    <p>${this.description}</p>
                    <!-- Add more content about volcanoes and awareness here -->
                </body>
            </html>
        `;
    }
}

// Usage Example for VolcanoWebsite

// Create a new instance of VolcanoWebsite
const myVolcanoWebsite = new VolcanoWebsite(
    "Volcano Awareness",
    "Welcome to our website about volcanoes and awareness. Learn about the different types of volcanoes, their impact on the environment, and how to stay safe during volcanic eruptions."
);

// Generate the HTML content for the website
const websiteContent = myVolcanoWebsite.generateWebsiteContent();

// Display the generated HTML content
console.log(websiteContent);
