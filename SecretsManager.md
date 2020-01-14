## secretsmanager

    aws secretsmanager describe-secret --secret-id MyTestDatabaseSecret
    
## to get Secret 

    aws secretsmanager get-secret-value --secret-id MyTestDatabaseSecret --version-stage AWSPREVIOUS
