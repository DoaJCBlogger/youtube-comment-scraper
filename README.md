YouTube Comment Scraper
=======================

## About
This is the web client for my Youtube Comment Scraper project. It is written in **Node.js** and uses the [**youtube-comment-api**](https://github.com/philbot9/youtube-comment-api) module to gain access to the comments.
Given a YouTube video URL the client will request all comments for that video from the API. The results are displayed as nicely formatted JSON and CSV and can also be downloaded in those formats.

The results include the following information:

* Comment ID
* Username
* Date
* Timestamp
* Number of Likes
* Comment Text
* Replies

To see it in action go to: [ytcomments.klostermann.ca](http://ytcomments.klostermann.ca)

## Dependencies
A number of third party resources are required and need to be placed in the indicated directories.

| Name | Directory |
|------|-----------|
| [jQuery](https://jquery.com/) | static/libs/jquery.min.js |
| [Font Awesome](http://fontawesome.io/) | static/font-awesome |
| [Bootflat](http://bootflat.github.io/) | static/bootflat |
| [Papa Parse](http://papaparse.com/) | static/libs/papaparse.min.js |
| [json.human.js](https://github.com/marianoguerra/json.human.js) | static/libs/json.human.js, static/libs/json.human.css |
| [download.js](http://danml.com/#/download.html) | static/libs/download.js |

## Deployment
The project includes a Dockerfile and deploy script. Running `./deploy` will create a new Docker image and deploy the node application in a container. The application will be listening for incoming connections on `http://localhost:49161`.


## Licensing
**youtube-comment-scraper** is licensed under ISC. See the included LICENSE file for details.

**This project is in no way affiliated with YouTube.**
