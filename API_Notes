SOAP
	is an xml-based design that has standardized structures for requests and responses.
REST
	Uses JSON
	Stands for:
		Representational
		State
		Transfer
	Is a more open approach providing lots of conventions but leaving many decisions to architect
	
	
REST
	DAO
		Data access layer
			provides an interface to connect with the database and access the data stored in the database
			a single dao class can deal with queries retrieving different types of entities
	Repository
		Layer that connects to the database and accesses data, similar to dao
		difference is that repository layer provides a greater abstraction compared to dao
		every class is responsible for accessing and manipulating one entity
	Service
		This layer calls the dao layer to get data and perform business logic
		The business logic in the service layer could be:
			Performing calculations on data recieved,
			Filtering data based on logic
	Model
		Contains all the java objects that will be mapped to the database table 
		dao will fetch the data from the database and populate the respective modell with that data and return it
		to the service layer and vice versa
	Controller
		top-most layer
		called when a request comes for a particular REST api
		the controller will process the rest api request, calls one or more services and returns an http response
		to the client

HTTP
	Request Headers:
		Accept: informs the server about the type of data that the client accepts
			example:
				Accept text/html
				Accept: Application/xhtml+xml
				Accept: image/png
		Accept-Encoding: Informs the server about the type of encoding the client can take
			example:
				Accept-Encoding: gzip
				Accept-Encoding: gzip, compress
		Authorization: is used to pass credentials for authentication and provide access where necesary
			example:
				Authorization: Basic YWxhZGRpbjpvcGVuc2VzYW1l
				Authorization: Bearer eyYWxhZGRpbjpvcGVuc2VzYW1l
		Accept-Language: self-explanatory
			example:
				Accept-Language: fr-CH
				Accept-Language: en-US
		Cache-Control: hoilds caching instruction for the client and server
			example:
				Cache-Control: stale-while-revalidate=60
				Cache-Control: no-cache
	Representation Headers: Contains metadata found in the body
		Content Type: defines the media type of the sources before any encoding
		Content-Encoding: used to decode message payloads
			Uses lossless compression methods
		Content-Language: Language
		Content Location: Shows the working directory for the response
	Payload Headers:
		Content-Length: indicates the size of the message body in bytes.
		Content-Range: indicates the position of a partial message in a full body message
		
IDEMPOTENT:When multiple calls of an http method yield the same result and leaves the server in the same state
	GET, HEAD, PUT, AND DELETE should be idempotent methods
	GET, HEAD, POST, AND PATCH ARE CACHEABLE for later used
	
REQUESTS:

	
