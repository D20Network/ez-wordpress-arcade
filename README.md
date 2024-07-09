# ez-wordpress-arcade

HTML5 Game Embedder
The HTML5 Game Embedder plugin allows you to embed HTML5 games on your WordPress website, track user statistics, and display games in an interactive slider. It provides a user-friendly interface for managing games, categories, and game details.

Features
Embed HTML5 games using an iframe code
Categorize games into different categories
Display game descriptions and thumbnails
Track user statistics like total play time and number of plays
Interactive game slider for browsing and selecting games
Leaderboard to display top users based on play time or number of plays
Installation
Upload the html5-game-embedder folder to the /wp-content/plugins/ directory, or install the plugin through the WordPress plugins screen directly.
Activate the plugin through the 'Plugins' screen in WordPress.
Usage
Adding a New Game
Go to the 'Games' menu in the WordPress admin area.
Click on 'Add New' to create a new game.
Enter the game title, description, and select a featured image (thumbnail).
In the 'Game Iframe Code' meta box, paste the iframe code for embedding the HTML5 game.
Assign the game to one or more categories using the 'Game Categories' taxonomy.
Publish the game.
Displaying Games
Use the following shortcodes to display games on your WordPress pages or posts:

[html5_game_embedder id="123"]: Displays a single game with the specified ID. Replace 123 with the actual game ID.
[html5_game_embedder_category_list category="action-games"]: Displays a list of games in the specified category. Replace action-games with the slug of the desired category.
[html5_game_embedder_slider category="action-games" limit="10" orderby="title" order="ASC"]: Displays an interactive game slider with up to 10 games from the "Action Games" category, ordered alphabetically by title in ascending order. You can customize the category, limit, orderby, and order parameters as needed.
[html5_game_embedder_leaderboard limit="20" order_by="total_plays" order="DESC"]: Displays a leaderboard with the top 20 users sorted by total plays in descending order. You can customize the limit, order_by, and order parameters as needed.
Tracking User Statistics
The plugin automatically tracks user statistics like total play time and number of plays for each game. This data is stored in a custom database table and can be displayed using the [html5_game_embedder_leaderboard] shortcode.

Uninstalling the Plugin
When you uninstall the HTML5 Game Embedder plugin, it will automatically remove the custom database table used for storing user statistics. However, it will not delete any games, categories, or other data created by the plugin.

Support
If you encounter any issues or have questions about the plugin, please reach out to us for support

Changelog
1.2
Added an interactive game slider with the [html5_game_embedder_slider] shortcode
Added a leaderboard feature with the [html5_game_embedder_leaderboard] shortcode
Implemented user statistics tracking for total play time and number of plays
Added an uninstall hook to remove the custom database table when the plugin is uninstalled
1.1
Added support for game categories
Implemented the [html5_game_embedder_category_list] shortcode to display games by category
1.0
Initial release
Added support for embedding HTML5 games using an iframe code
Implemented the [html5_game_embedder] shortcode to display individual games
