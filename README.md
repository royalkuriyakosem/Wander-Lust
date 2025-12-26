# WanderLust

WanderLust is a full-stack web application inspired by Airbnb, designed to help users discover and book unique accommodations around the world. It allows users to browse listings, view detailed information, read reviews, and manage their own property listings.

## Features

- **Browse Listings:** Users can view a wide variety of accommodations with images, descriptions, and pricing.
- **Detailed Views:** Click on any listing to see full details including location, host information, and amenities.
- **User Authentication:** Secure signup and login functionality using Passport.js.
- **Listing Management:** Registered users can create, edit, and delete their own listings.
- **Reviews & Ratings:** Users can leave reviews and ratings for listings they have visited.
- **Image Upload:** Integrated with Cloudinary for seamless image uploads and storage.
- **Map Integration:** (If applicable) Visual representation of listing locations.

## Tech Stack

- **Frontend:** HTML, CSS, Bootstrap, EJS (Embedded JavaScript templating)
- **Backend:** Node.js, Express.js
- **Database:** MongoDB (using MongoDB Atlas for production)
- **Authentication:** Passport.js (Local Strategy)
- **Image Storage:** Cloudinary
- **Validation:** Joi (Server-side validation)

## Prerequisites

Before running this project, ensure you have the following installed:

- Node.js (v18.17.1 or higher recommended)
- MongoDB (running locally or a cloud instance like MongoDB Atlas)

## Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/wanderlust.git
    cd wanderlust
    ```

2.  **Install dependencies:**
    ```bash
    npm install
    ```

3.  **Set up environment variables:**
    Create a `.env` file in the root directory and add the following configuration:
    ```env
    ATLASDB_URL=your_mongodb_atlas_connection_string
    SECRET=your_session_secret_key
    CLOUD_NAME=your_cloudinary_cloud_name
    CLOUD_API_KEY=your_cloudinary_api_key
    CLOUD_API_SECRET=your_cloudinary_api_secret
    ```

4.  **Run the application:**
    ```bash
    node app.js
    ```
    Or if you have `nodemon` installed:
    ```bash
    nodemon app.js
    ```

5.  **Access the app:**
    Open your browser and navigate to `http://localhost:8080`.

## Directory Structure

- `controllers/`: Logic for handling requests (Listings, Reviews, Users).
- `models/`: Mongoose schemas (Listing, Review, User).
- `routes/`: Express routes defining API endpoints.
- `views/`: EJS templates for rendering the frontend.
- `public/`: Static assets (CSS, JS, images).
- `utils/`: Helper functions and error handling classes.
- `init/`: Database initialization scripts.

## License

This project is licensed under the ISC License.
