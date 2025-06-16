
# Social Media Data Analysis with Bluesky API

**Author:** *Stephen Bouchardon*

This project lets you analyze the Bluesky social media activity on a certain topic.
Follow the instructions below to use the project:

##  Step 1 : Setup a Bluesky account

To access the Bluesky API, you need to register on the social media : https://bsky.app.

Please, do not share your credentials to **anyone**. These are private and should be only viewed by yourself !

Copy and paste the following commands in the terminal:
  ```bash
    cd bluesky_api
    touch .env
    vim .env
  ```
Edit the .env file:
Press i to enter insert mode and paste the content below.
```bash
    # .env
    BLUESKY_EMAIL="your_email@example.com"
    BLUESKY_PWD="your_password_here"
  ```
Then, press Esc, type :wq to save & exit the file.

Example:
```bash
    # .env
    BLUESKY_EMAIL="abc@gmail.com"
    BLUESKY_PWD="abc1234"
  ```

It is important to do this step correctly. Else, you will get an error and not be able to access the rest of the project.

## Step 2 : Launch the Jupyter Notebook

You should be able to login now through the Jupyter Notebook :
```bash
   jupyter notebook
   ```

Note that the Jupyter Notebook kernel's version is 3.10.5.

The project is located inside *main.ipynb*.

The main file automatically load the .env file and your credentials.
```python
   from dotenv import load_dotenv
   load_dotenv()
   ```

## Step 3 : Required Python modules 

The first cell shows you all the modules required for the project.

If you are using pip3 to install the modules:
```bash
   pip3 install atproto python-dotenv pandas textblob matplotlib numpy
   ```

- Name: atproto, Version: 0.0.61, Link to documentation: [https://docs.bsky.app/docs/get-started](https://docs.bsky.app/docs/get-started)
- Name: python-dotenv, Version: 1.0.0, Link to documentation: [https://saurabh-kumar.com/python-dotenv/](https://saurabh-kumar.com/python-dotenv/)
- Name: pandas, Version: 2.0.2, Link to documentation: https://pandas.pydata.org/docs/
- Name: textblob, Version: 0.19.0, Link to documentation: https://textblob.readthedocs.io/en/dev/
- Name: matplotlib, Version: 3.7.2, Link to documentation: https://matplotlib.org/stable/users/index.html
- Name: numpy, Version: 1.21.6, Link to documentation: https://numpy.org/doc/stable/
  
*The other modules used are Python's built-in standard libraries.*

Now, you are ready, enjoy !
