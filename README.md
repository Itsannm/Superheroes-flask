# Superheroes-flask
Flask API Documentation
This is a Flask API that provides endpoints to manage heroes and powers. It allows you to retrieve information about heroes and powers, update power descriptions, and create hero-power relationships.
Installation
Clone the repository:
bash

Copy

   git clone https://github.com/your-username/your-repo.git
Install the required dependencies:
bash

Copy

   pip install -r requirements.txt
Set up the database:
bash

Copy

   flask db init
   flask db migrate
   flask db upgrade
Usage
To start the Flask server, run the following command:
bash

Copy

flask run
The API will be accessible at http://localhost:5000.
Endpoints
Get all heroes
URL: /heroes
Method: GET
Response: List of all heroes
Get a hero by ID
URL: /heroes/{id}
Method: GET
Parameters:
id (integer): ID of the hero
Response: Information about the hero with the specified ID
Get all powers
URL: /powers
Method: GET
Response: List of all powers
Get a power by ID
URL: /powers/{id}
Method: GET
Parameters:
id (integer): ID of the power
Response: Information about the power with the specified ID
Update a power
URL: /powers/{id}
Method: PATCH
Parameters:
id (integer): ID of the power
Request Body:
description (string): Updated description of the power
Response: Updated information about the power
Create a hero-power relationship
URL: /hero_powers
Method: POST
Request Body:
strength (string): Strength of the hero-power relationship (must be one of: Strong, Weak, Average)
power_id (integer): ID of the power
hero_id (integer): ID of the hero
Response: Information about the hero with the newly created hero-power relationship
Swagger UI Documentation
You can access the Swagger UI documentation for this API at http://localhost:5000/api/docs. It provides a user-friendly interface to explore and test the API endpoints.
License
This project is licensed under the MIT License. See the LICENSE file for more information.
