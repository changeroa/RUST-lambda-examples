# 1. Create a new project
```bash
cargo lambda new new-lambda-project \
    && cd new-lambda-project
```

# 2. Serve the function locally for testing (runs in port number 9000 in default)
```bash
cargo lambda watch
```

# 3. Test Lambda function
```bash
cargo lambda invoke --data-ascii "{ \"command\": \"hi\" }"
```

# 4. build Lamabda funtion
```bash
cargo lambda build --release --arm64
```

# 5. Deploy the function on AWS Lambda
```bash
cargo lambda deploy
```
    Requirements:
        - requires AWS credentials

# 6. Debugging
```bash
--verbose
```


