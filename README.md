# Meetup auto-RVSP
A Python script that automatically confirms your attendance in your [Meetup](https://meetup.com) groups' upcoming events.

# Problem Statement
Write a program for meetup.com that sends an auto-RVSP to specific groups. For example, suppose you are a member of 7 different Meetup groups, some of which have very popular events that fill up quickly. You want to sign up for them as fast as possible to ensure that you get a spot.

Your program needs take care of authentication, searching for events in configured groups (not all), and automatically signing up on the user's behalf in a timely manner. Usage of existing Meetup client libraries is permitted.

# Prerequisites

- [Chrome WebDriver](https://chromedriver.chromium.org/),
- [Selenium](https://pypi.org/project/selenium/).

# Instructions

- Clone and navigate into the repository directory:

```bash
git clone https://github.com/akshansh2000/meetup-auto-rsvp.git
cd meetup-auto-rsvp/
```

- Change your **email** and **password** in the given `config.json` file:

```json
{
  "email": "<YOUR EMAIL ID>",
  "password": "<YOUR PASSWORD>"
}
```

- Run the script:

```bash
python3 meetup.py
```

The script will check for any new event in your joined groups every *30 minutes*, and automatically confirm your attendance for that event. It **will** notify you upon any confirmation, and also if no upcoming events are found.

---

This program is tested on **Ubuntu 20.04.4 LTS 64-bit** system.
