SHEENA MAE D RAFANAN 4-A

# JSON POST with Database Integration

The JSON POST API endpoint facilitates the transfer of structured data from the client to the server, allowing records to be created or modified. The request body facilitates the transmission of JSON data, making it flexible and suitable for transparent manipulation. Once processing is complete, the server provides an HTTP status code along with the requested JSON data. This technology is capable of supporting user registration, data updates and personalized processes while ensuring secure authentication. It is essential to consult the appropriate documentation for necessary endpoint specifications  and error handling protocols.

## API Description

An Application Programming Interface, commonly known as an API, is a foundational concept in software development. It serves as a bridge that allows different software systems to communicate and interact with one another. APIs provide a well-defined set of rules and protocols that enable developers to access specific features, functions, or data from a service, library, or platform, without needing to understand the internal workings of the system. APIs are used extensively in web development, mobile app development, and many other software contexts, facilitating the integration of external services, data sources, and libraries, which ultimately enhances the functionality, scalability, and efficiency of software applications. 

## Purpose:

The use of API (Application Programming Interface) is intended to enable software systems to interact and share data or functionality, allowing developers to access and integrate services and resources. and external  data into their applications, helping to improve functionality, promote interoperability, and speed development.

## Key Features:

Data Access and Integration: 

-APIs allow access to external data sources, enabling applications to retrieve and integrate data from various platforms and services.

Security: 

- Implements authentication and authorization mechanisms to control access and protect sensitive data and functions.

Authentication and Authorization:

- Implement secure user authentication and authorization mechanisms to protect your API endpoints.
- Fine-grained access control to restrict user actions based on roles and permissions.

Real-time Communication:

- Enable real-time communication between users with features like instant messaging, notifications, and live updates.
- WebSockets and other protocols for efficient real-time data exchange.

Data Management:

- Easily store, retrieve, and manage data using our API. It supports various data types and formats, ensuring compatibility with different systems.
- Secure data transmission and storage protocols to safeguard sensitive information.
  
Scalability and Reliability:

- Enable applications to scale by leveraging external services and resources, enhancing flexibility and performance.
- Redundancy and failover mechanisms to ensure uninterrupted service even in case of server failures.

Documentation and Support:

- Comprehensive API documentation with detailed endpoints, request methods, and response formats.
- Dedicated customer support to assist you in API integration, issue resolution, and updates.

Customization:

- Customize API endpoints and functionalities according to your specific use case and business requirements.
- Flexible configuration options to adapt the API to your application's unique needs.

Error Handling:

- Clear and concise error messages to facilitate easy debugging and troubleshooting.
- Predictive error handling to preemptively address potential issues.

## API Endpoints

http://127.0.0.1/api/public/postName

Function: This endpoint is designed to add new information to the database.
Required Parameters: First name (fname), Last name (lname).

http://127.0.0.1/api/public/postUpdate

Function: This endpoint is utilized for modifying existing data in the database.
Required Parameters: ID, First name (fname), Last name (lname).

http://127.0.0.1/api/public/postPrint

Function: This endpoint serves the function of displaying the data stored in the database.
Required Parameters: None.

http://127.0.0.1/api/public/postDelete

Function: This endpoint is responsible for removing specific data from the database.
Required Parameters: ID.


## Request Payload

## JSON Payload postName:

- Request payload:
{
  "lname":"hortizuela",
   "fname":"manny"
}

This payload is used for creating a new name entry. It requires both the last name ("lname") and first name ("fname") of the person being added.

## JSON Payload printName:
 
- Request payload:

This payload does not contain any specific fields. It might be used for retrieving or printing a name from the system.

## JSON Payload updateName:

- Request payload:
{
  "id":1,
  "lname":"wick",
   "fname":"john"
}

This payload is used for updating an existing name entry identified by the specified "id". It requires the updated last name ("lname") and first name ("fname") of the person.

## JSON Payload deleteName:

- Request payload:
{
  "id":1
}

This payload is used for deleting a name entry based on the specified "id". It only requires the unique identifier of the name entry to be deleted.

## Response

## JSON Payload postName:

- Response payload:
{
         "status":"success","data":null
}

"status": Indicates the status of the API request. In this case, it's "success" indicating that the request was successful.
"data": This field is present but set to null, indicating that no specific data is returned for successful postName requests.

## JSON Payload printName:

- Response payload:
{
         "status":"success","data":["lname":"hortizuela","fname":"manny","lname":"licayan","fname":"arnold"]
}

"status": Indicates the status of the API request. It's "success" indicating that the request was successful.
"data": An array containing objects, each representing a name entry. Each object contains "lname" (last name) and "fname" (first name) fields with corresponding values. The response includes multiple name entries.


## JSON Payload updateName:

- Response payload:
{
         "status":"success","data":null
}

"status": Indicates the status of the API request. It's "success" indicating that the request was successful.
"data": This field is present but set to null, indicating that no specific data is returned for successful updateName requests.


## JSON Payload deleteName:

- Response payload:
{
         "status":"success","data":null
}

"status": Indicates the status of the API request. It's "success" indicating that the request was successful.
"data": This field is present but set to null, indicating that no specific data is returned for successful deleteName requests.


## Usage

Follow these steps to manipulate database information using Postman and the API endpoints:

1. Launch Postman:
Ensure that Postman is installed and operational on your system.

2. Send a POST Request to Insert Data:
To insert data into the database via the /api/public/postName endpoint:

Choose the HTTP method as POST.
Input the URL: http://127.0.0.1/api/public/postName.
Within the request body, specify the parameters fname and lname along with the desired values for insertion.
Click "Send" to dispatch the request.

3. Send a POST Request to Update Data:
To update existing database entries using the /api/public/updateName endpoint:

Select the HTTP method as POST.
Enter the URL: http://127.0.0.1/api/public/updateName.
In the request body, include the parameters id, fname, and lname, along with the updated values.
Click "Send" to submit the request.

4. Send a POST Request to Print Data:
To showcase database data using the /api/public/printName endpoint:

Opt for the HTTP method as POST.
Specify the URL: http://127.0.0.1/api/public/printName.
Keep the request body empty as no additional parameters are required.
Click "Send" to transmit the request.

5. Send a POST Request to Delete Data:
To remove data from the database through the /api/public/deleteName endpoint:

Set the HTTP method to POST.
Enter the URL: http://127.0.0.1/api/public/deleteName.
In the request body, include the parameter id with the ID of the data you intend to delete.

Click "Send" to initiate the request.


## License

No License 


## Contributors

Sir Manny Hortizuela
provided:

- some codes
- database structure
- payloads
- etc.


## Contact
Include contact
information for inquiries or support.

Sheena Mae D. Rafanan
- heenamae.rafanan@student.dmmmsu.edu.ph
- 09516781365

