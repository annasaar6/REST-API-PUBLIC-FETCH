# REST-API-PUBLIC-FETCH

# Reflection

This assignment gave me a much better understanding of how Flask applications interact with external APIs and how important it is to understand the structure of the JSON data being returned. At first, I thought the changes would mainly involve swapping one URL for another, but I quickly learned that different APIs organize their data differently. I had to examine the NHTSA API response, identify where the actual records were stored, and then update the filtering logic to work with the new data structure.

One thing that surprised me was seeing that the vehicle data was nested inside a "Results" object instead of being returned directly as a list. Because of that, I had to adjust my code before the filter would work correctly. As the project progressed, the code evolved from working with healthcare provider information to filtering vehicle safety system data.

Testing was also an important part of the process. After making the changes, I ran the Flask application and accessed the `/items` endpoint to verify that only records with a `GroupName` of "Active Safety System" were returned. Seeing the filtered results displayed correctly helped confirm that the API request and filtering logic were working as expected.

Overall, I now have a stronger understanding of REST APIs, JSON parsing, Flask routes, and data filtering in Python. In the future, I would like to learn more about building my own APIs and adding more advanced filtering options for users.
