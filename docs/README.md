#!/usr/bin/env python3

"""
Dashboard application for users.
"""

from flask import Flask, render_template
from user_dashboard.config import Config

app = Flask(__name__)
app.config.from_object(Config)

from user_dashboard import routes

if __name__ == "__main__":
    app.run(debug=True)