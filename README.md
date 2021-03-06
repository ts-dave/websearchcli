# Web Search CLI
Web Search CLI is a command line utility written in Python that takes a string as an argument, opens the browser and searches for the string using search engine of choice.

The program also copies string from clipboard if no string argument is passed in command line. It supports multiple search engines (google, duckduckgo, yandex, and bing), allows user to choose which one to use via command line argument. Program defaults to google if no search engine in specified or search engine not supported.

## Prerequisites
* python >= 3.7
* click == 7.1.2
* pyperclip

## Installing and using WebSearchCLI

Installation:

* clone repository
    ```git clone <link>```
* change directory into project folder
    ```cd websearchcli```
* run setuptools in development mode
    ```pip install --editable .```


Usage:

    search --engine bing --text "hello world"
    
    or
    
    search -e bing -t "hello world"

If no search engine or text is specified, program opens google search as default search engine and searches for last text copied to clipboard.

Eg:

```search``` will open google and search for text in clipboard.

```search --text "hello world"``` 
 or
```search -t "hello world"``` will open google and search for "hello world" since no search engine is specified.

```search --engine duckduckgo``` 
or
```search -e duckduckgo```
will search duckduckgo with last text copied to clipboard as search parameter.

>Default search engine: Google

>Default text: copies from clipboard

## Contributing to WebSearchCLI
To contribute to WebSearchCLI, follow these steps:

1. Fork this repository.
2. Create a branch: git checkout -b <branch_name>.
3. Make your changes and commit them: git commit -m '<commit_message>'
4. Push to the original branch: git push origin <project_name>
5. Create the pull request.
6. Alternatively see the GitHub documentation on [creating a pull request](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request).

## Contributors
* [@ts-dave](https://github.com/ts-dave)

## Contact
You can contact me via email at [emsonjunior@gmail.com](emsonjunior@gmail.com).

## License
This project uses the [MIT License](https://opensource.org/licenses/MIT)
