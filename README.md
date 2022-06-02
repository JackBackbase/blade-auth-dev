



docker-compose up -d


aws configure --profile local
local/local/ca-central-1
aws configure list --profile local
<!-- export AWS_PROFILE=local
export AWS_ACCESS_KEY_ID=local
export AWS_SECRET_ACCESS_KEY=local -->
alias dynamolocal='aws dynamodb --endpoint-url http://localhost:8001 --profile local'

dynamolocal help
dynamolocal list-tables
dynamolocal create-table --table-name LOCAL-IngestionRecord --attribute-definitions AttributeName=bncId,AttributeType=S --key-schema AttributeName=bncId,KeyType=HASH --billing-mode PAY_PER_REQUEST

dynamolocal scan --table-name LOCAL-IngestionRecord > file_name.json
dynamolocal describe-table --table-name LOCAL-IngestionRecord
dynamolocal get-item --table-name LOCAL-IngestionRecord --key '{ "bncId": {"S": "57D089A268BF40F3C3828201B64B4FB757D089A268BF40F3C3828201B64B4FB7"}}'



