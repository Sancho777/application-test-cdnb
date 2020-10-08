# Cialdnb Test - Application

Application that, given a list of website URLs as input, visits them and finds, extracts and outputs the websites’ logo image URLs and all phone numbers (e.g. mobile phones, land lines, fax numbers) present on the websites.

## Instructions

**1 - Download and extract the project files on your computer.**

**2 - Open your command line prompt and navigate to the project folder.**

Note: You need to have python installed on your computer.

**3 - On Windows create a virtual enviroment with this commands:**

```commandline
python -m venv myenv

myenv\Scripts\activate

pip install -r requirements.txt
```

The Command will install all the modules necessary for the execution of the system.

**4 - To execute the project, save a ".txt" file, in the project folder with the urls you want to search and execute, one per line without commas.**

**5 - Execute the application:**

```commandline
scrapy crawl cialdnb_spider -o info.json
```

You will be asked to name the file with the the website addresses, Ex: websites.txt.

After you do that the app will create a json file named info.json in the project folder with the scraped informations.

## Docker

If you want to use docker, just run the docfile to create the image

```commandline
docker build . -t image-name
cat your_file.txt | docker run -i image-name
```
