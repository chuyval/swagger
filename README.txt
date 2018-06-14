# Build Server code using yaml file
swagger generate server -f swagger_sample.yaml -A sample_app_name

# Generate Client Code


# Get packages needed
go get -u -f ./...

# Generate api document
# Can outpout several formats
swagger serve swagger-petstore.yaml # Default redoc
swagger serve swagger-petstore.yaml -F swagger