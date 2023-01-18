
[theme]
primaryColor="#3b62b7"
backgroundColor="#f5f9f9"
secondaryBackgroundColor="#86b7f1"
textColor="#052773"
 Simple Streamlit webserver application for serving developed classification
	models.
    Author: Explore Data Science Academy.
    Note:
    ---------------------------------------------------------------------
    Please follow the instructions provided within the README.md file
    located within this directory for guidance on how to use this script
    correctly.
    ---------------------------------------------------------------------
    Description: This file is used to launch a minimal streamlit web
	application. You are expected to extend the functionality of this script
	as part of your predict project.
	For further help with the Streamlit framework, see:
	https://docs.streamlit.io/en/latest/
"""


# Upcoming Movies
import streamlit as st
import joblib,os

# Trending
import pandas as pd

# Vectorizer
news_vectorizer = open("resources/tfidfvect.pkl","rb")
tweet_cv = joblib.load(news_vectorizer) # loading your vectorizer from the pkl file

# Load your raw data
raw = pd.read_csv("resources/train.csv")

  # Building out the "Contact Us" page
    if selected == "Contact Us":

        if selected == "Contact Us":
            with st.form("form1", clear_on_submit=True):
                name = st.text_input("Enter full name")
                email = st.text_input("Enter email")
                message = st.text_area("Message")

                submit = st.form_submit_button("Submit Form")

# Required to let Streamlit instantiate our web app.
if __name__ == '__main__':
    main()
# Recommended for you
def main():
