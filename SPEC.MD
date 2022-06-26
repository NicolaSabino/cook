# Specs

Specifications and requirements of the `.cook` file extension.

## General

- Each recipe file has the extension `.cook`
- The .cook extension can alternatively be replaced with `.food`, `.meal`, `.eat` or `.drink` to put the emphasis on the final product, but the inner structure of the file is the same and they are all treated in the same manner.
- The .cook file is a textual file containing a JSON complex object.
- The version is a string composed of three integer numbers, major, minor, and increment number, separated by a dot.
- All identifiers in a .cook file have to be in snake case 
    ```json
    {
        "identifier": "content",
        "another_identifier": "content",
        "yet_another_identifier": "content"
    }
    ```

## Structure

- Each file is composed of **mandatory** fields, **descriptive** fields, and **extra** fields
    - A mandatory field is a JSON object that has t stand against some validation rules, crucial for the integrity and functionality of the file.
    - A descriptive field is a JSON object that has to stand against some validation rules, that enrich the content  of the file
    - An extra field is a JSON object that does not stand against any validation rule. Is a piece of additional information that can be introduced to shape such a file to accommodate a  specific need.

### Mandatory fields

- Each file has to contain the `version` field
    - A version is a string characterized by a `MAJOR`, `MINOR`, and `PATCH` integer value separated by a dot.
        - an increase of the MAJOR number corresponds to a non-retro compatible change
        - An increase of the MINOR number corresponds to a retro compatible change
        - PATCH is commonly used for small changes and bug fixes are always retro compatible
- Each file has to contain the `encoding` field
    - The encoding field is a string field
- Each file has to contain the `name` field
    - The name field is a string with a minimum of 3 characters and a maximum of 60.
- Each file has to contain a list (JSON array) of `ingredients`
- An `ingredient` has to contain a `name` and `quantity`
  - The name is a string with minimum length of 3 characters and maximum length of 60 characters.