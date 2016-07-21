# Part4-GoogleSheets-gRPCAPI-Script-Docker
TThe docker compose bundle runs two containers:

1. grpc: Runs the Google Sheets gRPC Server and responsible for sharing the main.proto file using volumes 
2. script: Runs the test script to test the functionality of the above server
