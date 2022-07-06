# Environment management project
Docker reference
colima stop; colima start --cpu 6 --memory 12 --mount $HOME:w

Blade operations
mvn clean install -Pclean-database
mvn clean blade:run

Blade references
https://start.backbase.com/blade
https://github.com/Backbase/blade

Backbase repo
https://repo.backbase.com/


Trouble shooting References
https://community.backbase.com/documentation/ServiceSDK/latest/service_sdk_debugging
https://community.backbase.com/documentation/foundation_services/latest/troubleshooting

--logging.level.org.apache.http.wire=DEBUG
--logging.level.org.springframework.web.filter.CommonsRequestLoggingFilter=DEBUG


API spec references
https://artifacts.backbase.com/artifactory/specs/approval/approval-client-api-v2.2.2.yaml
https://developer.backbase.com/api/specs/approval/approval-client-api/2.2.2/operations/Approvals/getApprovals


Tokens

{
  "sub": "manager",
  "naf": 1650837597,
  "cnexp": true,
  "anloc": true,
  "anexp": true,
  "enbl": true,
  "exp": 1650754797,
  "iat": 1650751197,
  "rol": [
    "ROLE_USER",
    "ROLE_group_manager(MANAGER)"
  ],
  "jti": "dc204c92-e25b-49ed-80e2-dd576d2c3d36"
}




