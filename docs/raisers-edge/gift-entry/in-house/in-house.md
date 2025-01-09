# In House

## Gifts by Appeal

### 3PW Third Party Web

| Field                     | Value                                                                                 |
| ------------------------- | ------------------------------------------------------------------------------------- |
| `Account Involvement`     | Link Account Involvement (Not the 3PW Vehicle, except ActBlue)                        |
| `Acknowledgement`         | Do Not Acknowledge                                                                    |
| `Appeal`                  | 3PW                                                                                   |
| `Gift Constituent Code`   | Individual                                                                            |
| `Hard Credit`             | Donor, if known. `Anonymous` if not                                                   |
| `Letter Code`             | No Thank You Needed                                                                   |
| `Name on Check`           | 3PW Vehicle (Third-party vendor)                                                      |
| `Reference`               | Donation source                                                                       |

??? question "How to differentiate between 3PW, EMP, and MG?"

    Material for MkDocs only bundles selected plugins in order to keep the size
    of the official image small. If the plugin you want to use is not included,
    you can add them easily:

    === "Material for MkDocs"

        Create a `Dockerfile` and extend the official image:

        ``` Dockerfile title="Dockerfile"
        FROM squidfunk/mkdocs-material
        RUN pip install mkdocs-macros-plugin
        RUN pip install mkdocs-glightbox
        ```

    === "Insiders"

        Clone or fork the Insiders repository, and create a file called
        `user-requirements.txt` in the root of the repository. Then, add the
        plugins that should be installed to the file, e.g.:

        ``` txt title="user-requirements.txt"
        mkdocs-macros-plugin
        mkdocs-glightbox
        ```

    Next, build the image with the following command:

    ```
    docker build -t squidfunk/mkdocs-material .
    ```

    The new image will have additional packages installed and can be used
    exactly like the official image.