## Contributor License Agreement

By contributing to this repository, you agree to abide by the terms and conditions of the [LICENSE](/LICENSE).

## How to Contribute

Thank you for considering contributing to our project! We welcome contributions from the community to help improve and grow this project. Please follow the guidelines below to make the process smooth for everyone involved.

### Contribution Workflow

1. **Fork the Repository**: Start by forking this repository to your own GitHub account using the "Fork" button at the top-right corner of this page.

2. **Clone the Repository**: Clone your forked repository to your local machine using the following command, replacing `<your-username>` with your GitHub username:

   ```shell
   git clone https://github.com/<your-username>/all-about-apikey.git

3. **Add an API key information**: Create a folder using the apikey name, if there are spaces then replace them with `-` and use lowercase letters and inside the folder create another markdown file called `README.md`. And after that use this format
```
    # [Title Web](Link Documentation)

    ## Description

    ## __Example Request__
    * Curl
    ```
    Curl Request
    ```

    * Raw
    ```
    Raw Request
    ```

    ## __Response__
    * Success
    ```
    Response if succes
    ```
    * Error
    ```
    Response if error
    ```

    ## __Regex__
    ```
    Regex for checking the API
    ```

    ## __Example API key__

    ```
    API Key (You can blank this if you dont have example api key)
    ```
```

### Tips
- **DO NOT** add the actual API key to this repository, if you want to add an example API key, revoke the API key first
- If you don't know where to start, you can check this [repository](https://github.com/public-apis/public-apis)
