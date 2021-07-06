# Twinder

Twinder is an experimental self grouping chat platform.

Users and Rooms have an interest profile represented by a 39 dimensional vector.

The probability of a user joining a room is determine by a scoring metric.

We have tried the following metric function:

    score(user, room) = dot(profile(user), profile(room))

Run the app:

    gunicorn -b 0.0.0.0:80 app:app
