# This Python script gathers and visualizes Age of Empires II match data to reveal player preferences for different civilizations:
1. Fetches match history data for specific Age of Empires II players:

    Uses the requests library to make API calls to the Age of Empires II API.
    Retrieves recent match history data for a list of players defined in the USER_IDS_LIST.

2. Processes and filters the data:

    Extracts relevant information from the match history, including player aliases, civilizations used, match dates, ELO ratings, and match types.
    Filters the data to only include matches of types 8 and 9 (likely representing specific game modes).

3. Creates a pie chart for each player:

    Uses the pandas library to create a DataFrame to organize the filtered data.
    Employs plotly.express to generate pie charts visualizing the distribution of civilizations used by each player.
    Each pie chart is titled with the player's alias and labeled "Civ Distribution for [alias] in 2024".

