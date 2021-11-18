# News-API
## Built by [Barbara Mutindi](https://github.com/barbaramutindi/)

## Description
News-API is a web application that displays a list of various news sources. On choosing a news source, it will preview the top news articles of the day. Clicking a news article will redirect the user to read it fully from the news source. It achieves this by using the [News API](https://newsapi.org/).

The app can be viewed at [Heroku](https://barbaranewsAPI.herokuapp.com/)

## User Stories
As a user,I would like to:
* See various news sources
* Select the ones I prefer
* See the top news articles from that news source
* See the image, description and time the news article was created
* Click on an article and read it fully from the news source

## Specifications
| Behaviour | Input | Output |
| :---------------- | :---------------: | ------------------: |
| Display news sources | **On page load** | List of various news sources is displayed in a list |
| Display tabs with news by category | **On Tab link click** | Clickable links to open news based on category |
| Display articles from a news source | **Click a news source** | Redirected to a page with articles from the source |
| Display the preview of an article | **On page load** | Each article displays an image,description and publication date |
| To Read an entire article  | **Click an article** | Redirected to the news source's site to read the entire article |

## SetUp / Installation Requirements
### Prerequisites
* python3.8
* pip
* virtualenv

### Cloning
* In your terminal:

        $ git clone https://github.com/barbaramutindi/News-API.git
        $ cd News-API
        
## Running the Application
* Creating the virtual environment

        $ python3.8 -m venv --without-pip virtual
        $ source virtual/bin/env
        $ curl https://bootstrap.pypa.io/get-pip.py | python
* Installing Flask and other Modules

        $ python3.8 -m pip install flask
        $ python3.8 -m pip install flask-bootstrap
        $ python3.8 -m pip install flask-script
        
* Setting up the API Key

        To be able to gather article info from the News API you will need an API Key.

        * Visit https://newsapi.org/ and register for an API key.
        * In the root directory of the project folder create a file: start.sh
        * Insert the following info into it:

                export NEWS_API_KEY='<Your-Api-Key>'
                python3.8 manage.py server

        * Insert the API Key you received from News Api where <Your-Api-Key> is.
       
* To run the application, in your terminal:

        $ chmod +x start.sh
        $ ./start.sh

## Testing the Application
* To run the tests for the class files:

        $ python3.8 manage.py tests

## Technologies Used
* Python3.8
* Flask

## License & copyright
© Barbara Mutindi
Licensed under the [MIT License](LICENSE).